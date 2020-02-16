pipeline {
	agent any
	options {
		timestamps()
	}
	tools {
	    maven 'maven-3.6.3'
	}


	stages { 
	    stage('Build') {
	        
	        steps {
	            withMaven() {
	                sh 'mvn -B clean findbugs:findbugs package'
	            }

	        }

	    }

	    
	}

}