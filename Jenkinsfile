pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Doing docker build..'
		    sh 'docker build /var/lib/jenkins/workspace/docker-examples/ruby/.'
		    sh 'docker build /var/lib/jenkins/workspace/docker-examples/tomcat/.'
		    sh 'docker build /var/lib/jenkins/workspace/docker-examples/redis/.'
		    
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
