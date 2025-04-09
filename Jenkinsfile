@Library('jenkins-shared-library') _

pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git url: 'https://github.com/meghanavalluri02/jenkins-shared.git', branch: 'main'
            }
        }

        stage('Build') {
            steps {
                echo "Building the application"
                sh './gradlew build' // Replace with your actual build command if different
            }
        }

        stage('Running Shared Library') {
            steps {
                script {
                    commonBuild()
                }
            }
        }
    }
}

