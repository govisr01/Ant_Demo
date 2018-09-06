pipeline
{
	agent any
	stages{
		stage('Git') {
			steps{
			git 'https://github.com/govisr01/Ant_Demo.git'
			}
			}
		stage('Install') {
			steps{
			bat 'ant'
			}
			}
		stage('Deploy') {
			steps{
			sh 'cp -r "C:\\Program Files (x86)\\Jenkins\\workspace\\SBI\\Fixed\\dist\\AntExample.war" "C:\\Program Files\\Apache Software Foundation\\Tomcat 8.5\\webapps"'
			}
			}
		}
}
