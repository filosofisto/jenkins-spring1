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
                    echo 'Do here other initializations'
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
                    echo 'Pipeline finished'
                    echo 'Enjoy result'
                '''
            }
        }
    }
}

// /opt/maven/apache-maven-3.8.1/bin/