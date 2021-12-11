 pipeline {
    agent any


    stages {
        stage ("cloning"){
          steps{
                bin " git clone https://github.com/contentful/the-example-app.nodejs.git"
                
                }
        }
   stage ("istalation"){
          steps{
                bin "npm install"
                
                }
        }
         stage ("Deploy"){
          steps{
                bin " npm run start:dev &"
                
                }
        }
        stage ("test"){
          steps{
                bin "curl http://localhost:3000"
                
                }
        }
        
        } 
        
    
 }
