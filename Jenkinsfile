pipeline {
 // adding an agent is compulsory
 agent any
	stages {
	stage('checkout') {
	  steps {
	   git credentialsId: 'c04dfaa5-e4bc-4645-9352-f4bfcc73bf8b',
			url: 'https://github.com/mohanna-t/spring-petclinic.git'
	  }
	 }
	 stage('build') {
	  steps {
	   bat "Build.bat"
	  }
	 }
	}
}