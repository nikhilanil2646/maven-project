pipeline {
    agent any
   tools {
    maven 'maven-3.9.2' 
  } 
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'mvn clean install'
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
    }
}
