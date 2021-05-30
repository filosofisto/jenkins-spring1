pipeline {
    agent any
    tools {
        maven 'Maven'
        jdk 'JDK'
    }
    stages {
        stage('Initialization') {
            steps {
                sh '''
                    echo 'Pipeline starting'
                '''
            }
        }
        stage('Build') {
            steps {
                sh 'mvn -B clean package'
            }
        }
        stage('Deploy') {
            steps {
                sh 'mvn deploy'
            }
        }
        stage('Termination') {
            steps {
                sh '''
                    echo 'Pipeline finished'
                '''
            }
        }
    }
}

