
pipeline {
	 agent any
	    stages{
	    	stage('1-clone'){
	    		steps{
	    		checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: '01b44015-5552-4132-bee4-166dad8754a6', url: 'https://github.com/EngConstance/Project4.git']]])
	    		}
	    	}
	    	stage('2-constance.sh'){
			steps{
	    		 sh /var/lib/jenkins/hat/Project4/constance.sh
			}
	    
	    	}
	    
	}
}
