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
        echo 'we are here again'
        //start chrome "https://github.com/Nileshpateel/hello-world-new/blob/master/index.html" 
      }
    }
  }
}
