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
            sh 'wget -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash'
		
                }
                    
            }
            }
       stage('Build5'){
            steps{
                script{
            sh 'source ~/.bashrc'
		
                }
                    
            }
       
       
        }         
        stage('Build5s'){
            steps{
                script{
            sh 'nvm install v14.15'
		
                }
                    
            }
       
       
        }
        
        
        
 }
 }
