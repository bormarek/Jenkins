pipeline {
    agent any

    stages {

        
        stage('Display Tree') {
            steps {
                script {
                    def treeCommand = isUnix() ? 'tree .' : 'cmd /c tree .'
                    bat(script: treeCommand, returnStatus: true)
                }
            }
        }

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
                sh 'tree /Users/marek/.jenkins/workspace/maven_test'
            }
        }
    }
}
