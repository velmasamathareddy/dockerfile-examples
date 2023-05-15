pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Doing docker build..'
		    sh 'docker build /var/lib/jenkins/workspace/docker-examples/maven/.'
		    
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
		}
        stage('Verification') {
            steps {
                echo 'Verification in progress....'
            }
        }
		stage('sending updtaes') {
            steps {
                echo 'sending updtaes....'
            }
        }
    }
}
