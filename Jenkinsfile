pipeline {
  agent any
  stages {
    stage('Deploy to S3') {
      steps {
        git url:'https://github.com/DmytroKyslyiNure/lab1.git', branch: "main"
        sh "aws s3 cp index.html s3://kislyi-bucket"
      }
    }
  }
}
