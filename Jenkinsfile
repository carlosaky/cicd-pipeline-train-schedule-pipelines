pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation (no-deamon flag is recomended in pipiline context)'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
