pipeline {
	agent any
	stages {
    	stage('First') {
        	steps {
            	sh 'env.VARIABLE="True"'
        	}
    	}
    	stage('Second'){
        	steps {
            	   when {
                	env.VARIABLE='stage('Second') ',
			value:'True'
            }
        	}
    	}
    	stage('Thrid') {
        	steps {
            	sh 'echo "Updating Second Stage"'
        	}
    	}
	}
}
