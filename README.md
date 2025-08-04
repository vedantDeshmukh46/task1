# task1

CI/CD Pipeline Implementation for React App on AWS using Azure  DevOps .I successfully implemented for the gym_webapp project, including deployment on AWS.
The application is a single-page frontend built using React.js. For hosting the live version, I used an EC2 instance on AWS, where I configured a Linux-based (Ubuntu) virtual machine.I also configured a self-hosted Azure DevOps agent on the EC2 instance so that it could run deployment jobs triggered by changes in the codebase.

Wrote a YAML-based pipeline in Azure DevOps that performs three key actions. First, it runs a npm install command to install all project dependencies. Next, it executes npm run build to compile the React project into static files. Finally, it clears the old files from the /var/www/html/ directory on the EC2 server and copies the newly built files into it.  
