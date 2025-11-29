This forked repository will be the source and starting point of our CI/CD pipeline, which will eventually compile and deploy the application on this repository on the EC2 instance. Here’s an overview of the files contained in the forked repository:

- **buildspec.yml**: This YAML file contains instructions on how to build the code in our application and how to package it into a deployment artifact.

- **appspec.yml**: This YAML file contains instructions on where to deploy the application and which scripts or hooks to run during deployment. In our appspec.yml file, we’ve defined commands to run the app_start.sh and app_stop.sh scripts.

- **app_start.sh**: This script contains the command to start our node application and will compile and start serving the application in the background.

- **app_stop.sh**: This script contains the command to stop our node application and will terminate any port on which a node application is being run.

- **web_app**: This is the directory of the Node.js project that we’ll be serving on our EC2 instance.
