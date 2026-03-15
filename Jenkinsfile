pipeline{
    agent any
    stages{
        stage('fetch code'){
            steps{
                git branch:'paac , '
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