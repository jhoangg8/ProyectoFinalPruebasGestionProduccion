pipeline {
  agent any
  stages {
    stage('PIPELINE2') {
      steps {
        sleep(time: 2, unit: 'MINUTES')
        build(job: 'JOB_3', propagate: true)
      }
    }

  }
}