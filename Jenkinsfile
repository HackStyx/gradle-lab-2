pipeline{
  agent any
  tools{
    gradle "Gradle"
    jdk "JDK"
  }
  stages{
  stage('checkout'){
    steps{
      git "https://github.com/HackStyx/gradle-lab-2.git"
    }
  }
    stage('build'){
      steps{
        sh 'gradle build'
      }
    }
    stage('run'){
      steps{
        sh 'gradle run'
      }
    }
  }
}
