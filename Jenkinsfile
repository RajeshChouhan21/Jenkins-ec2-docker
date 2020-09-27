pipeline {
    agent none

    stages {
        stage('Build') {
            agent { label 'ec2-slave' }
            steps {
                echo 'Building..'
                sh '''pwd
                '''
            }
        }
    }

}
