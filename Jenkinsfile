pipeline {
  agent any
  stages {
    stage ('Build'){
      steps {
        echo 'Running build automation'
	sh './grandlew build --no-daemon'
	ArchiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}