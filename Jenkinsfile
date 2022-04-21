pipeline {
      agent any
      stages {
            stage('Init') {
                      script {
                            properties([pipelineTriggers([pollSCM('* * * * *')])])
                        }
                        git branch: 'feature1', url: 'https://github.com/Prasanna7396/MultibranchJenkins.git'                  
                        steps {
                              echo 'Hi, this is Prasanna'
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
