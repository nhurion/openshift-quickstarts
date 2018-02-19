pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        readMavenPom(file: 'undertow-servlet/pom.xml')
        echo 'hello'
      }
    }
    stage('install') {
      steps {
        build 'install'
      }
    }
  }
}