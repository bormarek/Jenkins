pipeline {
    agent any

    stages {
        stage('Step 1') {
            steps {
                echo 'Executing Step 1'
		git 'https://github.com/bormarek/java_example.git'
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
            }
        }
    }
}
