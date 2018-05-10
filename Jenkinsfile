pipeline {
  agent any
  stages {
    stage('1st stage') {
      parallel {
        stage('1st stage') {
          steps {
            sleep 10
            echo 'hogehoge'
          }
        }
        stage('1st stage 2') {
          steps {
            echo 'ooooops'
          }
        }
      }
    }
    stage('2nd stage') {
      steps {
        echo 'do mvn!'
      }
    }
  }
}