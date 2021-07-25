pipeline {
    agent any

    options{
        skipDefaultCheckout()
    }

    stages {
        stage('SCM') {
            steps {
                checkout scm
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}