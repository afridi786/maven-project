pipeline{
	 agent any
	stages{
	stage('scm checkout'){
	steps{
	git 'https://github.com/afridi786/maven-project.git'
	}
	}
	stage('compile code'){
	steps{
	withMaven(jdk: 'LOCAL_JDK', maven: 'LOCAL_MAVEN') 
   {
	sh 'mvn compile'
	}

	}
	}
	}
	
}
