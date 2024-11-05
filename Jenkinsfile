pipeline {
    agent any
    stages {
        stage('checking root') {
            steps {
            sh 'ls -al'
            sh 'pwd'
            }
        }

        stage('checking src') {
            steps {
                dir('src') { // Assume 'src' contains your application code
                    sh 'ls -al'

                }
            }
        }

        stage('dependencies') {
            steps {
                dir('test') { // Navigate to the dependencies directory
                    sh 'ls -al'
                    // Example: run tests or scripts related to dependencies
                    // e.g., sh './dependency1/test.sh'
                }
            }
        }
    }
}
