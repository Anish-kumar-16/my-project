pipeline{
  agent any

  stages{
    stage('Build'){
      tools{
        maven 'Maven-3'
      }
      steps{
        sh 'mvn clean package -DskipTests'
      }
    }
    stage('Docker Build'){
          steps{
            sh 'docker build -t student-app:1.0 .'
          }
    }
  }
}
