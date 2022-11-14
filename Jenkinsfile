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
            sh 'wget -o- https://deb.nodesource.com/setup_16.x -o /tmp/nodesource_setup.sh'
		
                }
                    
            }
            }
       stage('Build5'){
            steps{
                script{
            sh 'sudo bash /tmp/nodesource_setup.sh'
		
                }
                    
            }
       
       
        }         
        stage('Build5s'){
            steps{
                script{
            sh 'sudo apt install nodejs'
		
                }
                    
            }
       
       
        }
        
        
        
 }
 }
