pipeline {
  agent any
  stages {
    stage('sonarqube') {
      steps {
        withSonarQubeEnv(installationName: 'sonar', credentialsId: '1234', envOnly: true) {
          findBuildScans()
        }

      }
    }

  }
}