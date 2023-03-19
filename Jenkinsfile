pipeline {
	agent any
	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/vboxuser/Downloads/apache-maven-3.9.0/bin/mvn install'
	                 }}
		stage('Deployment'){
		    steps {
			
			sh 'cp target/snapdeal.war vboxuser@127.0.1.1:/home/vboxuser/Downloads/apache-tomcat-9.0.71/webapps'
	}
}}}
