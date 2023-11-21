pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                script {
                    sh "git config --global user.name 'dipali-coditas'"
                    sh "git config --global user.email 'dipali.dhanwade@coditas.com'"
                    sh "chown jenkins:jenkins /home/dipali_dhanwade/script.sh"
                    sh "chmod +x /home/dipali_dhanwade/script.sh"
                    sh "bash /home/dipali_dhanwade/script.sh"
                }
            }
        }
    }
}

