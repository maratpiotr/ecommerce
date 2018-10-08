pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean install'
        cleanWs(deleteDirs: true, cleanupMatrixParent: true, cleanWhenUnstable: true, cleanWhenSuccess: true, cleanWhenNotBuilt: true, cleanWhenFailure: true, cleanWhenAborted: true)
      }
    }
  }
}