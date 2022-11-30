pipeline {
    agent any
        stages {
            stage ('compile stage') {

                steps {
                        sh 'maven clean compile'
                  
                }
            }
             stage ('Testing stage') {

                steps {
                
                        sh 'maven test'
                    
                }
            }
            stage ('Deploy stage') {

                steps {
                    
                        sh 'maven deploy'
                    
                }
            }
        }
}
