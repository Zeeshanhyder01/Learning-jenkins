//
//pipeline {
//    agent { label 'MY-WORKSTATION' }
//
//    stages {
//
//        stage('TEST01') {
//            steps {
//                echo'TEST01'
//            }
//        }
//
//        stage('TEST02'){
//            steps {
//                echo'TEST02'
//            }
//        }
//
//        }
//    post {
//        cleanup {
//            echo" Hi This is demo of jenkins post conditions"
//        }
//
//        always {
//            echo" Hi This is demo of jenkins post  always conditions"
//        }
//
//        fixed {
//            echo" Hi This is demo of jenkins post fixed conditions"
//        }
//    }
//    }


pipeline {
    agent any

    environment{
        SAMPLE_URL="GOOGLE.COM"
        MY_CREDENTIALS = credentials('SSH CONNECTION')
    }

    stages {
        stage('One'){
            steps {
                sh 'echo URL=${SAMPLE_URL}'
                echo SAMPLE_URL
                echo MY_CREDENTIALS
            }
        }

    }
}
//declarative doesnt allow to read dynamic varaibles at stage so go with scripted ppl
//
//env.SAMPLE_URL="GOOGLE.COM"
//node{
//    stage("one - ${SAMPLE_URL}"){
//        echo SAMPLE_URL
//
//    }
//}