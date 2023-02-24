pipeline {
  agent any

  stages {
    stage('Clone Git repository') {
      steps {
        git 'https://github.com/Nileshpateel/hello-world-new'
      }
    }
    
    stage('Copy HTML file to workspace') {
      steps {
        bat 'copy index.html $WORKSPACE'
      }
    }
    
    stage('Open HTML file in web browser') {
      steps {
        bat 'start http://localhost:8090/index.html'
      }
    }
  }
}
