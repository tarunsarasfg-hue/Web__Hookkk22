pipeline {
  agent any
  triggers { githubPush() }
  stages {
    stage('Build') {
      steps { sh 'sh build.sh' }
    }
    stage('Test') { 
      steps { sh 'sh test.sh' }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying to staging' }
    }
