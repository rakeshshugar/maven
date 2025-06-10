pipeline {
    agent any

    tools {
        maven 'maven'  // Maven installation name configured in Jenkins
    }

    stages {
        stage("Clean") {
            steps {
                sh 'mvn clean'
            }
        }

        stage("Compile") {
            steps {
                sh 'mvn compile'
            }
        }

        stage("Test") {
            steps {
                sh 'mvn test'
            }
        }

        stage("Package") {
            steps {
                sh 'mvn package'
            }
        }
    }
}
