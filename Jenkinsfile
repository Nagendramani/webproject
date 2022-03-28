pipeline {
  agent any
  stages {
    stage ("build docker image") {
      steps {
        sh 'sudo docker build -t nagendramani/webapp:1.0 . '
      }
    }
    stage ("push to repo"){
      steps {
        sh ' sudo docker login -u nagendramani -p Saibaba@5'
        sh 'sudo docker push nagendramani/webapp:1.0'
        
      }
    }
  }
}
