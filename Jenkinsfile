pipeline
{
agent any
stages {
stage(‘Pull’) {
steps{
script{
checkout([$class: 'GitSCM’, branches: [[name: '*/main’]],
userRemoteConfigs: [[
credentialsId: 'GithubCred',
url: ‘https://github.com/Ghassenmoalla/Myapp.git']]])
}
}
}
}
}
