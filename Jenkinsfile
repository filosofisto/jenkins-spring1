pipeline {
    agent any
    tools {
        maven 'Maven'
        jdk 'JDK'
        sonarScanner 'SonarScanner'
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
//                 sh 'mvn -B clean package'

                   sh 'echo ${sonarScanner}'
//                 sh '/var/lib/jenkins/sonarqube-scanner/sonar-scanner-4.6.2.2472/bin/sonar-scanner'
//                 sh 'sh ${tool("Sonar")}/bin/sonar-scanner \
//                     -Dsonar.projectKey=jenkins-spring1 \
//                     -Dsonar.sources=./src/main/java \
//                     -Dsonar.host.url=http://3.121.215.50:9000 \
//                     -Dsonar.login=cc06e2f526f7b00de5eaf3dd9824e9e4c18c2f11'
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

