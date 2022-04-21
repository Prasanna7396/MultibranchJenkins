pipeline {
      agent any
      stages {
            stage('Init') {
                  steps {
                      script {
                            properties([pipelineTriggers([pollSCM('* * * * *')])])
                        }
                        git branch: 'main', url: 'https://github.com/Prasanna7396/MultibranchJenkins.git'
                        echo 'Hi, this is Prasanna Jadhav'
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
             stage('QA') {
                  steps {
                        echo "QA Testing a few cases"
                  }
            }
            stage('Deployment') {
                  steps {
                        echo "Deploying in Deployment Area"
                  }
            }
      }
}
