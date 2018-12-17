pipeline {
  agent any
  stages {
    stage('Received an event') {
      steps {
        sh 'echo \'I just received a buildCompleted event\''
      }
    }
  }
  triggers {
    eventTrigger(simpleMatch('buildCompleted'))
  }
}