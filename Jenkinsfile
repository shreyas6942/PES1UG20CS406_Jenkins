pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'g++ -o PES1UG20CS406 PES1UG20CS40612.cpp'
      }
    }
    stage('Test') {
      steps {
        sh './PES1UG20CS406-1'
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo "Deployment Step"'
      }
    }
  }
  post {
    
  
    failure {
      echo 'Pipeline failed'
    }
  }
}
