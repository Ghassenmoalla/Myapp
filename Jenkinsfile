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
            sh 'sudo npm install --force'
            sh 'ansible-playbook Ansible/build.yml -i Ansible/inventory/host.yml'
		
                }
                    
            }
            }

        
        
        
 }
 }
