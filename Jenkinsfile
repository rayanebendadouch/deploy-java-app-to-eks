pipeline{
agent : any
tools {
maven 'maven3'
}
stages{
stage('checkout'){
git branch:'master', CredentialsId:'github', url:'https://github.com/rayanebendadouch/deploy-java-app-to-eks.git'
}
stage('build'){
sh 'mvn clean package'
}
stage('test'){
sh 'mvn test'
}
}


}
