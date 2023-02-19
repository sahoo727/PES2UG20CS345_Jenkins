pipeline {
    agent any

stages{
  stage('Build') {
    steps{
      sh 'i++ -o PES2UG20CS345 PES2UG20CS345.cpp'
    }
  }

  stage('Test') {
    steps{
       sh './PES2UG20CS345'
    }
  }

  stage('Deploy') {
    steps{
      echo 'Deployment successful'
    }
  }
}
post {
    failure {
        echo 'Pipeline Failed'
    }
  }
}
