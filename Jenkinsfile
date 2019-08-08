pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        withAWS(region:'us-east-2', credentials: 'IDofSystemCredentials') {
          s3Upload(file:'index.html', bucket:'jenkinsudacityseiya', path:'/')
        }
      }
    }
  }
}