@Library('commonLib') _
pipeline {
    agent any

    stages {
        stage('Build and Deploy') {
            steps {
                script {
                    commonBuild()
                }
            }
        }
    }
}
