pipeline {
  agent any
  stages {
    stage('PIPELINE2') {
      steps {
        sleep(time: 2, unit: 'MINUTES')
        build(job: 'JOB_3', propagate: true)
        withSonarQubeEnv(installationName: 'SonarQube', credentialsId: '1695a12e7267a762e085824cc7464120d0002689', envOnly: true) {
          echo 'Sonar OK'
        }

      }
    }

  }
}