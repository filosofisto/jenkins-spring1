pipeline {
    agent any
    tools {
        maven 'Maven'
        jdk 'JDK'
    }
    stages {
        stage('Build') {
            steps {
                sh '/opt/maven/apache-maven-3.8.1/bin/mvn -B clean package'
            }
        }
    }
}