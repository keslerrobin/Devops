pipeline {
  agent none
  stages {
    stage('Test') {
      steps {
        sh 'run test'
      }
    }

    stage('build') {
      steps {
        build(job: '1', propagate: true, quietPeriod: 1)
      }
    }

  }
  environment {
    Test = '1'
    ok = '0'
  }
}