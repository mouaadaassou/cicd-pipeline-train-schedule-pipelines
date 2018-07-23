pipeline {
  agent any;
  stages {
    stage ('Build the project') {
      steps {
        sh './gradlew build --no-daemon'
        sh 'pwd && ls -larth'
        archiveArtifacts artifacts: 'dest/result.zip'
      }
    }
  }
}
