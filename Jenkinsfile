pipeline {
    agent  {
        label 'AGENT-1'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    post {
        always {
            echo "Success"
        }
        success{
            echo "Success"
        }
        failure {
            echo "Failure"
        }
    }
}