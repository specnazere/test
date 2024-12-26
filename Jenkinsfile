pipeline {
    agent any
    stages {
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