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
            }
        }
        stage('test'){
            steps{
                sh 'this si test stage'
            }
        }
        stage('deploy'){
            steps{
                sh 'this is deploy stage'
            }
        }
    }
}