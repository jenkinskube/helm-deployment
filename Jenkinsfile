pipeline
{
  agent { label 'slave3' }
    stages {

 stage('Git-Checkout') {
steps {
echo "Checking the git repo";
git branch: 'main', url: 'https://github.com/jenkinskube/helm-deployment.git'
sh 'ls -l'

}
}
stage('Echo output'){
steps{
sh 'echo $NODE_NAME'
sh 'echo "Executing next command"'
sh 'hostname'
sh 'echo "SUCCESS"'

}
}
}
}
