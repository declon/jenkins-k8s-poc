pipeline {
  agent {
    kubernetes {
      label 'python'  // all your pods will be named with this prefix, followed by a unique id
      idleMinutes 5  // how long the pod will live after no jobs have run on it
      yamlFile 'BuildContainers.yaml'  // path to the pod definition relative to the root of our project 
      defaultContainer 'python3'  // define a default container if more than a few stages use it, will default to jnlp container
    }
  }
  stages {
    stage('Build') {
      steps {
        sh "python --version"   
      }
    }
  }
}
