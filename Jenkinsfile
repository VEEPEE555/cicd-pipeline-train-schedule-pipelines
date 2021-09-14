pipeline{
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running Buld automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    } 
  }
}
