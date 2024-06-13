pipeline {
    agent {
        label 'MAMATHA'
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh '''
                echo 'hi from webhook'
                '''
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
            echo 'I will always run whether job is success or not'
        }
        success{
            echo 'I will run only when job is success'
        }
        failure{
            echo 'I will run when failure'
        }
    }
}