pipeline {
    agent any

    options{
        skipDefaultCheckout()
    }

    stages {
        stage('SCM') {
            steps {
                script {
                    try {
                        input 'Deploy to UAT?'
                    } catch (err) {
                        currentBuild.result = 'SUCCESS'
                    }
                }
            }
        }
    }
}