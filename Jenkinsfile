pipeline {
	agent any
	stages {
    	stage('First') {
        	steps {
            	sh 'env.berejob="True"'
        	}
    	}
    	stage('Second'){
        	steps {
            	   when {
                	echo ${berejob}:'berejob ',
			value:'True'
            }
        	}
    	}
	}
}
