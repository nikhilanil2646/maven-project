pipeline {
    agent none
   tools {
    maven 'maven-3.9.2' 
  } 
    stages {
        stage('Build') {
	agent any
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
	agent {label 'ubuntu'}
            steps {
                echo 'Deploying....'
		sh 'scp -r dist user@server:/var/www/temp_deploy/dist/'

            }
        }
    }
}
