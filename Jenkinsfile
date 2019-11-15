pipeline {
	agent any
	stages {
    	stage('First') {
        	script {
            	  env.berejob="True"
        	}
    	}
    	stage('Second'){
        	script{
            	   when {
                	environment name: 'berejob',
			value:'True'
            }
        	}
    	}
	}
}
