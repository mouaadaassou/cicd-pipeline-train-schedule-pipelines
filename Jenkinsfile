pipeline {
  agent any;
  stages {
    steps('Build the project') {
      sh './gradlew build --no-daemon'
      archiveArtifacts artifacts: 'dest/result.zip'
    }
  }
}
