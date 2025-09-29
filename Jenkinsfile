pipeline{
agent any
tools {
maven 'maven3'
}
stages{
stage("checkout"){
steps{
git branch: 'master', CredentialsId: 'github', url: 'https://github.com/rayanebendadouch/deploy-java-app-to-eks.git'
}
}
stage("build"){
steps{
sh 'mvn clean package'}
}
stage("test"){
steps{
sh 'mvn test'}
}
}


}
