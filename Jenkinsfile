pipeline {
  agent any
  stages {
    stage('pull') {
      steps {
        git(url: 'https://github.com/Pavel-Eliav/test-webpage.git', branch: 'master', poll: true)
      }
    }
    stage('test') {
      steps {
        sh 'find index.html'
      }
    }
  }
}