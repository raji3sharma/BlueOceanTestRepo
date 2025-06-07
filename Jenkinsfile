pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Building the code'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'testing the code'
          }
        }

        stage('testing_parellel') {
          steps {
            echo 'Parellel test is running'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'Deployement done'
      }
    }

  }
}