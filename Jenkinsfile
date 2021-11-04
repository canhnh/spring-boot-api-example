pipeline {
    agent any

    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                sh 'chmod +x ./gradlew build'
            }
        }
        stage('Test') {
            steps {
                sh 'chmod +x ./gradlew test'
            }
        }
    }
}