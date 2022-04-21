pipeline {
      agent any
      stages {
            stage('Init') {
                  steps {
                         script {
                            properties([pipelineTriggers([pollSCM('H/1 * * * *')])])
                         }
                         git branch: 'feature2', url: 'https://github.com/Prasanna7396/MultibranchJenkins.git'
                        
                         echo 'Hi, this is Prasanna'
                  }
            }
            stage('Build') {
                  steps {
                        echo 'Building Sample Maven Project'
                  }
            }
            stage('Testing') {
                  steps {
                        echo "Testing a few cases"
                  }
            }
            stage('Deployment') {
                  steps {
                        echo "Deploying in Deployment Area"
                  }
            }
      }
}
