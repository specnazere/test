pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                // Клонируем репозиторий с использованием учетных данных
                git branch: 'main', url: 'https://github.com/specnazere/test.git', credentialsId: 'github-credentials'
            }
        }
        stage('Read index.html') {
            steps {
                script {
                    // Читаем содержимое файла index.html
                    def content = readFile('index.html')
                    // Выводим содержимое в консоль
                    echo content
                }
            }
        }
    }
}