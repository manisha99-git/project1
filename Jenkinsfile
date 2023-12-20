pipeline {
	agent any
	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/manisha/Documents/MAVENMAIN/extraction/apache-maven-3.9.3/bin/mvn install'
	                 }}
		stage('Deployment'){
		    steps {
			
		sh 'cp target/project1.war /home/manisha/Documents/MAVENMAIN/extraction/apache-tomcat-9.0.76/webapps'
	}}
}}
