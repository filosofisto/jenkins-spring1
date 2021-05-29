pipeline {
    agent any
    tools {
        maven 'Maven'
        jdk 'JDK'
    }
    stages {
        stage('Source') {
            checkout('https://github.com/filosofisto/jenkins-spring1')
        }
        stage('Build') {
            steps {
                withMaven(maven: 'Maven') {
                    sh 'mvn clean package'
                }
                //sh 'mvn -B clean package'
            }
        }
    }
}

// /opt/maven/apache-maven-3.8.1/bin/