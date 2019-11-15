pipeline {
	agent any
	stages {
    	stage('First') {
        	steps {
            	  env.berejob="True"
        	}
    	}
    	stage('Second'){
        	steps{
		 sh 'echo "Step Three"'
        	}

                 when {
                        environment name: 'berejob',
                        value:'True'
            }
    	}
	}
}
