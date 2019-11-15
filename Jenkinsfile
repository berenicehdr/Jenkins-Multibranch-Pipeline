pipeline {
	agent any
	stages {
    	stage('One') {
        	steps {
            	sh 'echo "Step One"'
        	}
    	}
    	stage('Two'){
        	steps {
            	sh 'make check'
            	junit 'echo "Step Two"'
        	}
    	}
    	stage('Three') {
        	steps {
            	sh 'echo "Step Three"'
        	}
    	}
	}
}
