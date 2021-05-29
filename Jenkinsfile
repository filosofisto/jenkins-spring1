pipeline {
    agent any
    tools {
        maven 'Maven'
        jdk 'JDK'
    }
    stages {
        stage('Source') {
            git url: 'https://github.com/filosofisto/jenkins-spring1'
        }
        stage('Build') {
            steps {
                sh 'mvn -B clean package'
            }
        }
    }
}

// /opt/maven/apache-maven-3.8.1/bin/