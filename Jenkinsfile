pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://github.com/muntaser4github/blueocean-test-repo.git', branch: 'master', credentialsId: 'github')
      }
    }

    stage('Build') {
      steps {
        sh 'mvn compile'
      }
    }

  }
}