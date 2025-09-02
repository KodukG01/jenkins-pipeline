pipeline {
    agent {
        label 'roboshop-dev'
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
            echo "Say hello"
            deleteDir()
        }
        success{
            echo "pipeline is success"
        }
        failure{
            echo "pipeline is failure"
        }

    }
}