pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Check website file') {
            steps {
                script {
                    if (!fileExists('index.html')) {
                        error('index.html was not found')
                    }
                }
                echo 'Website file exists. Basic check passed.'
            }
        }
    }
    post {
        success { echo 'My Study Planner pipeline passed.' }
        failure { echo 'Build failed. Check Console Output.' }
    }
}
