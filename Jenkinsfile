pipeline {
  agent any
  stages {
    stage ('Build'){
      steps {
        echo 'Running build automation'
	sh './grandlew build --no-daemon'
	archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}