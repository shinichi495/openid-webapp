pipeline {
    agent any

    tools {
            maven 'maven3'
            jdk 'jdk-8'
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean install'
                sh 'mvn jetty:run-war'
            }
        }

    }
}