pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        echo 'This is step 1'
        echo 'this is step2'
      }
    }

    stage('stage2') {
      parallel {
        stage('stage2') {
          steps {
            echo 'this is step1 from stage2'
          }
        }

        stage('stage2A') {
          steps {
            echo 'this is step1 from stage 2A'
          }
        }

      }
    }

    stage('stage3') {
      steps {
        echo 'this is step 1 from  stage3'
      }
    }

  }
}