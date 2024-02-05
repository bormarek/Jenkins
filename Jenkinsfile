pipeline {
    agent any

    stages {

        stage('Step 1') {
                steps {
                    cleanWs()
                    echo 'Executing Step 1'
                    sh 'git clone https://github.com/bormarek/java_example.git'
                }
            }

            stage('Step 2') {
                steps {
                    echo 'Executing Step 2'
                    sh 'ls -ltr'
                }
            }
        
        stage('Step 3') {
            steps {
            echo 'Executing Step 3'
                sh 'ls -ltr /Users/marek/.jenkins/workspace/maven_test'
            }
        }
    }
}
