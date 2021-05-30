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
                    echo 'Release pipeline starting'
                '''
            }
        }
        stage('Build') {
            steps {
                sh 'mvn -B -Dmaven.test.skip=true clean package'
            }
        }
        stage('Termination') {
            steps {
                sh '''
                    echo 'Release pipeline finished'
                '''
            }
        }
    }
}

