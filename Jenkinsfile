pipeline {
  agent any
  tools{
    maven "Maven"
  }
  environment{
    NEW_VERSION = '1.3.0'
  }
  stages {
    stage('Build') {
      steps {
        echo 'Building verison $(NEW_VERSION)..'
        sh "nvm install"
        // Here you can define commands for your build
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
