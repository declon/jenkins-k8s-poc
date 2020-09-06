pipeline {
  agent {
    kubernetes {
      yamlFile 'BuildContainers.yaml'
    }
  }
  stages {
    stage('Python') {
      steps {
        container('python3') {
          sh "python ./script.py"
        }
      }
    }
    stage('Ubuntu') {
      steps {
        container('ubuntu') {
          sh "python ./script.sh"
        }
      }
    }
  }
}
