pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Doing docker build..'
		    sh 'docker build /var/lib/jenkins/workspace/docker-examples/ubuntu/.'
		   // sh 'docker build /var/lib/jenkins/workspace/docker-examples/tomcat/.'
		   // sh 'docker build /var/lib/jenkins/workspace/docker-examples/redis/.'
		    
            }
        }
        stage('Tagging') {
            steps {
                echo 'Doing Docker Tagging..'
		 sh 'docker tag komljen/ubuntu:latest velmasamatha123/myubuntu:latest'
            }
        }
        stage('Docker Push to dockerhub') {
            steps {
                echo 'Docker push to docker hub....'
	        sh 'docker push velmasamatha123/myubuntu:latest'
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
