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
          sh '''
             python ./script.py
             cat /etc/os-release
          '''
        }
      }
    }
    stage('Ubuntu') {
      steps {
        container('ubuntu') {
          sh '''
	     ./script.sh
             cat /etc/os-release
	  '''
        }
      }
    }
  }
}
