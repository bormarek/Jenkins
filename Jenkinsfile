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
    }
}
