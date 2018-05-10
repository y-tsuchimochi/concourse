pipeline {
  agent any
  stages {
    stage('1st stage') {
      parallel {
        stage('1st stage') {
          steps {
            sleep 10
            echo 'hogehoge'
            sh 'ls -lR'
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
    stage('3rd stage') {
      steps {
        script {
          def date = new Date()
        }

      }
    }
  }
}