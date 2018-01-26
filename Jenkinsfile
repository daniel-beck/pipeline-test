pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mkdir -p foo .svn ; touch foo/bar .svn/WTF'
        archiveArtifacts artifacts: '*/', defaultExcludes: false, onlyIfSuccessful: true
      }
    }
  }
}
