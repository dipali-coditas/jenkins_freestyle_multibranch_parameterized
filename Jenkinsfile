pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                script {
                  dir("/var/lib/jenkins/workspace/Test") {
                        // Change to the desired working directory

                        // Ensure correct ownership and permissions for the Jenkins workspace
                        sh "sudo chown -R jenkins:jenkins ."

                        // Clone the specific branch from the Git repository
                        sh "rm -rf websitedevelopmenttt"
                        sh "git clone -b main --single-branch https://github.com/dipali-coditas/websitedevelopmenttt.git"
                        
                        // Change to the cloned repository directory
                        dir("websitedevelopmenttt") {
                            // Ensure correct ownership and permissions for script.sh
                            sh "sudo chown jenkins:jenkins script.sh"
                            sh "chmod +x script.sh"

                            // Execute the script
                            sh "bash script.sh"
                }
            }
        }
    }
}


