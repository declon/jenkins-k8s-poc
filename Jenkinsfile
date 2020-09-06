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
          sh "python --version"   
        }
      }
    }
  }
}
