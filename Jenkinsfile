pipeline {
  agent any;
  stages {
    stage ('Build the project') {
      steps {
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dest/result.zip'
      }
    }
  }
}
