pipeline {
 // adding an agent is compulsory
 agent any
	stages {
	stage('checkout') {
	  steps {
	   git 'https://github.com/mohanna-t/spring-petclinic.git'
	  }
	 }
	 stage('build') {
	  steps {
	   bat "Build.bat"
	  }
	 }
	}
}