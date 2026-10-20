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


## Jenkins Pipeline Integration

This project uses Jenkins to check the website files automatically.

### Pipeline Setup

1. Open Jenkins at http://localhost:8080.
2. Create a new item named campus-event-hub-ci.
3. Select Pipeline as the job type.
4. Choose Pipeline script from SCM.
5. Select Git as the source control system.
6. Enter the repository URL:
   https://github.com/sarthak262006-design/campus-event-hub.git
7. Set the branch to */main.
8. Set the Script Path to Jenkinsfile.
9. Save the configuration and click Build Now.

### Checking Build Results

1. Open the latest build in Jenkins.
2. Click Console Output.
3. Check whether the build finishes with SUCCESS or FAILURE.

The pipeline checks out the repository and performs basic website file and content checks.
