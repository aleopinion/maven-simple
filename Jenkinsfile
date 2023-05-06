pipeline {
    agent any
    tools {
        maven "M3"
    }
    stages {
        stage ('Compile') {
            steps {
                sh "mvn clean compile"
            }
        }
        stage ('Test') {
            steps {
                sh "mvn clean test"
            }
        }

        stage ('Install') {
            steps {
                sh "mvn clean install"
            }
        }
    }
}