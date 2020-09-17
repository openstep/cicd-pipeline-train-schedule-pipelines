pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        atchiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
