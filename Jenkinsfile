pipeline {
  agent {
    node {
      label 'maven-build-server'
    }
  }

  tools {
    maven 'Maven-3.9.8'
  }

  stages {
    stage('Code Build Stage') {
      steps {
        sh 'mvn install -Dmaven.test.skip=true'
      }
    }
  }
}
