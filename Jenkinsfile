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
        
        echo 'Deployment completed'
      }
    }
    stage('Monitoring') {
      steps {
        
        echo 'Monitoring completed'
      }
    }
    stage('Dev') {
      steps {
       
        echo 'Dev completed'
      }
    }


    stage('Dev1') {
      steps {
       
        echo 'Dev completed'
      }
    }

    stage('Notify for new Bulid ') {
      steps {
        echo 'New JOb done '
      }
    }

  }
}