pipeline {
    agent any  // Runs the pipeline on any available agent

    stages {
        stage('Checkout Code') {
            steps {
                // Checkout the code from the GitHub repository
                git url: 'https://github.com/surajnikam0/hello-world.git', branch: 'main'  // Adjust the branch if needed
            }
        }

        stage('Hello World') {
            steps {
                echo 'Hello, World!'  // Prints "Hello, World!" in the Jenkins console
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished.'  // Always runs, regardless of success or failure
        }
    }
}


