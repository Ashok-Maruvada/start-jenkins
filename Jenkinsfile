pipeline{
    agent{
        label 'agent-1'
    }
    options {
        timeout(time: 30, unit: 'MINUTES')
        disableConcurrentBuilds()
    }
    stages{
        stage('build'){
            steps{
                echo 'this is build stage'
            }
        }
        stage('test'){
            steps{
                echo 'this si test stage'
            }
        }
        stage('deploy'){
            steps{
                echo 'this is deploy stage'
            }
        }
    }
}