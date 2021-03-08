pipeline {
  agent any
  stages {
    step ('Upload to AWS') {
      withAWS(region:'us-east-2',credentials:'aws-static') {
      s3Upload(pathStyleAccessEnabled:true, payloadSigningEnabled: true, file:'index.html', bucket:'myudacityproject21')
      }
    }
  }
}
