pipeline {
  agent any
  stages {
    stage('Pull SCM') {
      steps {
        echo 'SCM stage success'
      }
    }

    stage('Deploy_DEV & QA') {
      parallel {
        stage('Deploy_DEV') {
          agent any
          steps {
            echo 'DEV stage success'
          }
        }

        stage('Deply_QA') {
          agent any
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