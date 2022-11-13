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
                    sh "ansible-playbook ansible/build.yml -i ansible/inventory/host.yml"
                }
            }
       
        }         
        
        
        
        
 }
 }
