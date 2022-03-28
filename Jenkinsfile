pipeline {
  agent any
  stages {
    stage ("build docker image") {
      steps {
        sh docker build -t nagendramani/webapp:1.0
      }
    }
    stage ("push to repo"){
      steps {
        sh docker login -u nagendramani -p Saibaba@5
        sh docker push nagendramani/webapp:1.0
        
      }
    }
  }
}
