pipeline
{
agent any
stages {
	stage(‘Pull’) {
	steps{
	script{
	checkout([$class: 'GitSCM', branches: [[name: '*/main']],
	userRemoteConfigs: [[
	credentialsId: 'GithubCred',
	url: 'https://github.com/Ghassenmoalla/Myapp.git']]])}
      	      }
	    
	   }
	   
	stage('Build'){
            steps{
                script{
            sh "curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh 
| bash"
                }
                
                   script{
            sh "nvm install node"

                }
                
            }
       
        }         
        
        
        
        
 }
 }
