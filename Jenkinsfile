pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running Jenkins build stage in pipeline'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
