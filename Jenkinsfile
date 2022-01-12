pipeline {
  agent any
  stages {
    stage('Docker Build') {
      steps {
         sh 'docker build -t abdallauno1/mysba:latest .'
      }
    }
    stage('Docker Push') {
      steps {
        withCredentials([usernamePassword(credentialsId: 'dockerHub', passwordVariable: 'dockerHubPassword', usernameVariable: 'dockerHubUser')]) {
          sh "docker login -u ${env.dockerHubUser} -p ${env.dockerHubPassword}"
          sh 'docker push abdallauno1/mysba:latest'
         }
      }
    }
  }
}