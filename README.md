# mynodeJSapp

### The first step to getting this code is to clone it by running the command below:
- git clone https://github.com/TechDom-Ca/mynodejsapp.git
- You need to have ***git*** installed on the server


### Install npm or nodejs, then run either of the following:
- npm login 
- npm adduser

### Once you have npm or nodejs installed, run the following commands:
- cd mynodejsapp
- npm install

### Start the application by running either of the following:
- node app.js
- npm start

### To run test cases, run:
- npm test

### To generate a SonarQube report, run either of the following:
- npm run sonar
- node sonar-project.js

### To generate a Nexus token using base64 encoding:
- echo -n 'admin:enterYourPassword' | openssl base64

### Create a .npmrc file in the project root directory and add the following lines:

  registry=<<NexusRepoURL>>
  _auth=<<Token>>
  email=<<EmailID>>
  always-auth=true


### In package.json, add the following entry:

  "publishConfig": {
  "registry": "http://IPAddress:8081/repository/nodejs-repo/"
  }

### Then, run the following command to login to the Nexus repository:
- npm login --registry=NexusRepoURL
  
### Finally, use this command to upload packages to the Nexus repository:
- npm publish




npm publish
  
