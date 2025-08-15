pipeline {
    agent  {
        label 'AGENT-1'
    }
    environment {
        courrse = "Jenkins"
    }
    options {
        timeout(time: 30, unit: 'seconds')
    }

    stages {
        stage('Build') {
            steps {
                script {
                    echo 'Building..'
                    sh 'echo "Build step executed"'
                    
                }
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