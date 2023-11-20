pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                sudo chown jenkins:jenkins /home/dipali_dhanwade/script.sh
                sudo chmod +x /home/dipali_dhanwade/script.sh
                sudo bash /home/dipali_dhanwade/script.sh
            }
        }
    }
}
