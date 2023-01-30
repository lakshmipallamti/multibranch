pipeline {
 agent any
  environment {
    PATH="$PATH:/opt/maven3.8/bin" 
  }
  stages {
    stage('git') {
      steps {
        git'https://github.com/lakshmipallamti/multibranch.git'
      }
    }
    stage('build') {
      steps {
       sh 'mvn clean package' 
      }
    }
  }
}
