pipeline { 
 agent any 
 
 stages { 
 
  stage('Clone') { 
   steps { 
    git 'https://github.com/sambhramnaregal/ci-node-app-j.git' 
   } 
  } 
 
  stage('Install') { 
   steps { 
    bat 'npm install' 
   } 
  } 
 
  stage('Run App') { 
   steps { 
    bat 'node app.js' 
   } 
  } 
 
  stage('Test') { 
   steps { 
    bat 'npm test' 
   } 
  } 
 
 } 
}