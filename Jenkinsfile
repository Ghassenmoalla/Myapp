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
            sh ' npm install --force'
            sh 'ansible-playbook Ansible/build.yml -i Ansible/inventory/host.yml'
		
                }
                    
            }
            }
    stage('Docker'){
            steps{
                script{
            sh 'ansible-playbook Ansible/docker.yml -i Ansible/inventory/host.yml'
		
                }
                    
            }
            }
        
        
        
 }
 }
