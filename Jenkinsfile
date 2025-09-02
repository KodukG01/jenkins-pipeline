pipeline {
    agent {
        label 'roboshop-dev'
    }
    stages {
        stage('Build') {
            steps {
                script {
                     echo 'Building..'
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