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
                    echo 'Main pipeline starting'
                '''
            }
        }
        stage('Build') {
            steps {
                sh 'mvn -B clean package'
            }
        }
        stage('Termination') {
            steps {
                sh '''
                    echo 'Main pipeline finished'
                '''
            }
        }
    }
}

