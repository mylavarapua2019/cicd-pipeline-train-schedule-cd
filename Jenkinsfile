pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                echo %PATH%
                gradlew build --no-daemon
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
