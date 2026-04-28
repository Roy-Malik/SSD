pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Muhammad Ammar Shahid, 23i-2125, added to jenkins build step'        // Here you can define commands for your build
      }
    }
    stage('Test') {
      steps {
        echo 'Testing..'
        // Here you can define commands for your tests
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying....'
        // Here you can define commands for your deployment
      }
    }
  }
  post {
    always {
      echo 'Post building cond running'
    }
    failure {
      echo 'post action if build failed'
    }
  }
}
