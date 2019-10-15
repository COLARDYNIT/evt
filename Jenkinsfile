pipeline {
    agent any
    stages {
        stage('deploy: prd'){
            steps {
                echo "Deploying on PRD"
                sh "scp -r -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null site/* ubuntu@e-v-t.be:/data/www/evt/"
            }
        }
    }
}