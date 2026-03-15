pipeline{
    agent any
    stages{
        stage('fetch code'){
            steps{
                        git branch: 'main', url: 'https://github.com/Rocky-RS/jenkins-pipeline-peoject.git'
            }
        }
        stage('build'){
            steps {
                sh 'mvn install'
            }
        }
        stage('test'){
            steps{
                sh 'mvn test'
            }
        }
    }
}
