pipeline{
    agent{
        label 'agent-1'
    }
    options {
        timeout(time: 30, unit: 'MINUTES')
        disableConcurrentBuilds()
    }
    environment{
        DEPLOY_TO =  'production'
        GREETING = 'Good Morning'
    }
    stages{
        stage('build'){
            steps{
                sh 'echo this is build stage'
                sh 'env'
            }
        }
        stage('test'){
            steps{
                sh 'echo this is test stage'
            }
        }
        stage('deploy'){
            steps{
                sh 'echo this is deploy stage'
                sh 'this is ashok'
            }
        }
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
        success { 
            echo 'I will run when pipeline is success'
        }
        failure { 
            echo 'I will run when pipeline is failure'
        }
    }
}