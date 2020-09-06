pipeline {
  agent {
    kubernetes {
      yamlFile 'BuildContainers.yaml'
    }
  }
  stages {
    stage('Build') {
      steps {
        container('python3') {
          sh "python -c 'import os; print(os.getcwd()); print(\"Hello, Declon\")'"   
        }
      }
    }
  }
}
