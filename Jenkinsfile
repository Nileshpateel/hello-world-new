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
        sh 'cp index.html $WORKSPACE'
      }
    }
    
    stage('Open HTML file in web browser') {
      steps {
        sh 'xdg-open http://localhost:${env.8090}/index.html'
      }
    }
  }
}
