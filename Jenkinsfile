pipeline {
      agent any
      stages {
            stage('Init') {
                  steps {
                        echo 'Hi, this is Prasanna Jadhav'
                        echo 'We are Starting the Testing'
                  }
            }
            stage('Build') {
                  steps {
                        echo 'Building Sample Maven Project'
                  }
            }
            stage('Deploy in staging') {
                  steps {
                        echo "Testing a few cases"
                  }
            }
            stage('Deploy in Prod') {
                  steps {
                        echo "Deploying in Deployment Area"
                  }
            }
      }
}
