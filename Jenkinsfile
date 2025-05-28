pipeline {
  agent any

  tools {
    gradle 'Gradle' // Ensure "Gradle" is defined in Jenkins tool config
    jdk 'JDK'       // Ensure "JDK" is defined in Jenkins tool config
  }

  stages {
    stage('Checkout') {
      steps {
        git 'https://github.com/HackStyx/gradle-lab-2.git'
      }
    }

    stage('Build') {
      steps {
        sh './gradlew build' // Use wrapper if available
      }
    }

    stage('Run') {
      steps {
        sh './gradlew run'
      }
    }
  }
}
