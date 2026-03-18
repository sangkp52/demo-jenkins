pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/sangkp52/demo-jenkins.git'
            }
        }

        stage('Build') {
            steps {
                dir('demo') {
                    bat 'mvn clean package'
                }
            }
        }
    }
}