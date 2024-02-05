pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Pobierz kod źródłowy z systemu kontroli wersji (np. Git)
                git 'https://github.com/bormarek/Jenkins.git'
            }
        }

        stage('Display Message') {
            steps {
                // Wyświetl prosty komunikat
                echo 'Hello, Jenkins! This is a simple pipeline.'
            }
        }
    }
}

