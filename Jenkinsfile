pipeline {
  agent any
  stages {
    stage ('Pre-step') {
      steps {
        echo 'Running Pre-step' > abc.txt
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
