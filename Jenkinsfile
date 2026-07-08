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
        bat 'echo "building the app"'
      }
    }
    stage('Test'){
      steps{
        bat 'echo "running tests"'
      }
    }
    stage('Deploy'){
      steps{
        bat 'echo "deploying"'
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
