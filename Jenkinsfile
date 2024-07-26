pipeline {
  agent any
  stages {
    stage('Pull SCM') {
      steps {
        echo 'SCM stage success'
      }
    }

    stage('Deploy_DEV') {
      parallel {
        stage('Deploy_DEV') {
          steps {
            echo 'DEV stage success'
          }
        }

        stage('Deply_QA') {
          steps {
            echo 'QA stage success'
          }
        }

      }
    }

    stage('Deploy_Prod') {
      steps {
        echo 'Prod stage success'
      }
    }

  }
}