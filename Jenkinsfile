pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Completed '
      }
    }

    stage('Test') {
      parallel {
        stage('Test 2 ') {
          steps {
            echo 'Running Test 2'
          }
        }

        stage('Test one') {
          steps {
            echo 'runing test one'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        input(message: 'Are yoy to deploy', ok: 'Yes ')
        echo 'Deployment completed'
      }
    }

    stage('Notify for new Bulid ') {
      steps {
        echo 'New JOb done '
      }
    }

  }
}