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
            sh 'curl -sL https://deb.nodesource.com/setup_14.x | sudo -E bash -'
		
                }
                    
            }
       stage('Build'){
            steps{
                script{
            sh 'sudo apt install nodejs'
		
                }
                    
            }
       
       
        }         
        
        
        
        
 }
 }
