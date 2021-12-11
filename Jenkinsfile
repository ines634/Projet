pipeline {
    agent any


    stages {
        stage ("cloning"){
          steps{
                sh "git clone https://github.com/contentful/the-example-app.nodejs.git"
                
                }
        }
   stage ("istalation"){
          steps{
                sh "npm install"
                
                }
        }
         stage ("Deploy"){
          steps{
                sh "npm run start:dev &"
                
                }
        }
        stage ("test"){
          steps{
                sh "curl http://localhost:3000"
                
                }
        }
        
        } 
        
    
 }
 
 
