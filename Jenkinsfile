pipeline {
	agent any
	tools {
	maven 'MAVEN_HOME'
	}
	
	stages {
		
		stage ('Welcome Stage')
		{
			steps
				{
					echo 'Welcome to Jenkins Pipeline'
				}
		}
		
		stage ('Maven Clean')
		{
			steps
				{
					bat 'mvn clean'
				}
		}
		
		stage ('Maven Package')
		{
			steps
				{
					bat 'mvn package'
				}
		}
		
		stage ('Maven Install')
		{
			steps
				{
					bat 'mvn install'
				}
		}
		
		stage ('Final Build Stage')
		{
			steps
				{
					echo 'Build Done'
				}
		}
	}
}