pipeline {
    agent  {
        label 'AGENT-1'
    }
    environment {
        courrse = "Jenkins"
    }
     parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
        text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')
        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')
        choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password') 
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