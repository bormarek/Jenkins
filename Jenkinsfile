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
                    sh 'mvn clean package'
                }
            }
        
        stage('Step 3') {
            steps {
            echo 'Executing Step 3'
                sh 'ls -ltr /Users/marek/.jenkins/workspace/maven_test'
            }
        }
    }
    post {
        success {
            // Jeśli budowa zakończyła się sukcesem, wykonaj odpowiednie akcje
            echo 'Budowa zakończona sukcesem! Aplikacja została zbudowana poprawnie.'
            // Tutaj można dodać dodatkowe kroki, np. wdrożenie aplikacji
        }
        failure {
            // Jeśli budowa zakończyła się niepowodzeniem, wykonaj odpowiednie akcje
            echo 'Budowa zakończona niepowodzeniem! Sprawdź logi i popraw błędy.'
            // Tutaj można dodać dodatkowe kroki, np. powiadomienie o niepowodzeniu
        }
    }
}
