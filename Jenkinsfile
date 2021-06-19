pipeline {
  agent any
  stages {
    stage ('Pre-step') {
      steps {
        echo 'Running Pre-step'
        sh "echo 123 > abc.txt"
      }
    }
    stage ('Build') {
      steps {
        echo 'Running build automation'
        archiveArtifacts artifacts: 'abc.txt'
      }
    }
  }
}
