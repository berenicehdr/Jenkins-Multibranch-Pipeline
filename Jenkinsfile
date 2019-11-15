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
                	echo ${VARIABLE}:'VARIABLE ',
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
