pipeline {
	agent any
	stages {
    	stage('First') {
        	steps {
            	echo  env.berejob="True"
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
