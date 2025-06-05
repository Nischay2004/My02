pipeline {
  agent any
  tools {
    gradle 'Gradle'
    jdk 'JDK'
  }
  stages {
    stage('Checkout') {
      steps {
        git 'https://github.com/Nischay2004/My02.git'
      }
    }
      stage('Build') {
        steps {
          sh './gradlew build'
        }
      }
    stage('Test') {
      steps {
        sh './gradlew test'
      }
    }
    stage('Run Application') {
      steps {
        sh './gradlew run'
      }
    }
  }
}
