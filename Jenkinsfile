pipeline {
    agent any
        stages {
            stage ('compile stage') {

                steps {
                    withMaven(maven : '3.8.6') {
                        sh 'maven clean compile'
                    }
                }
            }
             stage ('Testing stage') {

                steps {
                    withMaven(maven : '3.8.6') {
                        sh 'maven test'
                    }
                }
            }
            stage ('Deploy stage') {

                steps {
                    withMaven(maven : '3.8.6') {
                        sh 'maven deploy'
                    }
                }
            }
        }
}