pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running automated build'
                sh './gradlew build'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}