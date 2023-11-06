pipeline {
	agent any 
	
	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/poonam/Documents/Devops/apache-maven-3.9.5/bin/mvn install'
	                 }}
		stage('Deployment'){
		   steps {
		sh 'cp target/sample-declarative.war /home/poonam/Documents/Devops/apache-tomcat-9.0.82/webapps'
			}}	
}}
