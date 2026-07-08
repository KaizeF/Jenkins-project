pipeline{
  agent any
  stages{
    stage('Checkout Code'){
      steps{
        git 'https://github.com/KaizeF/Jenkins-project'
        
      }
    }
    stage('Build'){
      steps{
        sh 'echo "building the app"'
      }
    }
    stage('Test'){
      steps{
        sh 'echo "running tests"'
      }
    }
    stage('Deploy'){
      steps{
        sh 'echo "deploying"'
      }
    }
  }
}
post{
  success{
    bat 'echo "build successful"'
  }
  failure{
    bat 'echo "build failed"'
  }
}
