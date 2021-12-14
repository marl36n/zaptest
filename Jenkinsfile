pipeline {
    agent any
    stages {
        stage('Baseline Scan') {
            steps {
				//deleting all files in the current workspace so we start clean
				cleanWs()
 
				       }
		
		stage('scan'){

			sh "docker-run -t owasp/zap2docker-stable zap-baseline.py -t http://www.newtours.demoaut.com/"
		}
        }
    }
 
}
