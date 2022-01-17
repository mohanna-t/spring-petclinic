pipeline {
 // adding an agent is compulsory
 agent any
	stages {
	stage('checkout') {
	  steps {
	   git branch:'main', 
		   credentialsId: 'c04dfaa5-e4bc-4645-9352-f4bfcc73bf8b',
		   url: 'https://github.com/mohanna-t/spring-petclinic.git'
	  }
	 }
	 stage('Build') {
	  steps {
	   //bat "Build.bat"
	   bat "set JAVA_HOME=C:\\Program Files\\Java\\jdk-17.0.1 "
	   bat "D:\\Mohanna\\Installer\\Maven\\apache-maven-3.8.4\\bin\\mvn compile"
	  }
	 }
	 
	 stage('Test') {
	  steps {
	   bat "set JAVA_HOME=C:\\Program Files\\Java\\jdk-17.0.1 "
	   bat "D:\\Mohanna\\Installer\\Maven\\apache-maven-3.8.4\\bin\\mvn test"
	  }
	 }
	 
	 stage('Package') {
	  steps {
	   bat "set JAVA_HOME=C:\\Program Files\\Java\\jdk-17.0.1 "
	   bat "D:\\Mohanna\\Installer\\Maven\\apache-maven-3.8.4\\bin\\mvn package"
	  }
	 }
	 
	}
}