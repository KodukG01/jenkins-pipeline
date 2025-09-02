pipeline {
    agent {
        label 'roboshop-dev'
    }
    environment{
        course = 'jenkins'
    }
    options {
        time(time: 1, unit: 'HOURS')
    }
    stages {
        stage('Build') {
            steps {
                script {
                    sh """
                     echo 'Building..'
                     env

                     """
                }
               
            }
        }
        stage('Test') {
            steps {
                script{
                    echo 'Testing..'
                }
            }
        }
        stage('Deploy') {
            steps {
               script{
                 echo 'Deploying....'
               }
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