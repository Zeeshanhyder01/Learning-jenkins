
pipeline {
    agent { label 'MY-WORKSTATION' }

    stages {

        stage('TEST01') {
            steps {
                echo'TEST01'
            }
        }

        stage('TEST02'){
            steps {
                echo'TEST02'
            }
        }

        }
    post {
        cleanup {
            echo" Hi This is demo of jenkins post conditions"
        }

        always {
            echo" Hi This is demo of jenkins post  always conditions"
        }

        regression {
            echo" Hi This is demo of jenkins post regression conditions"
        }
    }
    }