 pipeline {
    agent any


    stages {
        stage ("cloning"){
          steps{
           bat "[ -d 'the-example-app.nodejs' ] && rm -rf the-example-app.nodejs"
                bat " git clone https://github.com/contentful/the-example-app.nodejs.git"
                
                }
        }
   stage ("istalation"){
          steps{
           bat "cd the-example-app.nodejs" 
                bat "npm install"
                
                }
        }
         stage ("Deploy"){
          steps{
                bat " npm run start:dev &"
                
                }
        }
        stage ("test"){
          steps{
                bat "curl http://localhost:3000"
                
                }
        }
        
        } 
        
    
 }
