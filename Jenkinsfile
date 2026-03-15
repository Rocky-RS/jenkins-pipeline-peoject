pipeline {
    agent any

    tools {
        jdk 'jdk17'
        maven 'MAVEN3'
    }

    stages {

        stage('fetch code') {
            steps {
                git branch: 'main', url: 'https://github.com/Rocky-RS/jenkins-pipeline-peoject.git'
            }
        }

        stage('build') {
            steps {
                sh 'mvn clean install'
            }
        }

        stage('test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}



















