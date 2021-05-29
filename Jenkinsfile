pipeline {
    agent any
    tools {
        maven 'Maven'
        jdk 'JDK'
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B clean package'
            }
        }
    }
}