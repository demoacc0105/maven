pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/Naveen04jan/ven.git'
            }
        }

        stage('Build & Test') {
            steps {
                sh 'mvn -v'
                sh 'java -version'
                sh 'mvn clean install'
            }
        }

        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
