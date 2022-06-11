pipeline {
  agent any
  stages {
    stage('step 1') {
      parallel {
        stage('step 1') {
          steps {
            echo 'hi'
          }
        }

        stage('step 2') {
          steps {
            echo 'hi2'
          }
        }

      }
    }

    stage('finished') {
      steps {
        sh 'sh \'echo "done"\''
      }
    }

  }
  environment {
    env1 = 'qian'
  }
}
