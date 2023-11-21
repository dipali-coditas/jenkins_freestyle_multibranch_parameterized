pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                script {
                    sh "chown jenkins:jenkins /home/dipali_dhanwade/script.sh"
                    sh "chmod +x /home/dipali_dhanwade/script.sh"
                    sh "bash /home/dipali_dhanwade/script.sh"
                }
            }
        }
    }
}

