pipeline {
    agent any
    stages {
        stage('Read and Process File') {
            steps {
                script {
                    // Путь к файлу
                    def filePath = 'file.txt'
                    
                    // Читаем файл
                    def fileContent = readFile(filePath)
                    
                    // Вывод содержимого файла
                    echo "Содержимое файла:\n${fileContent}"
                    
                    // Сохранение содержимого в переменную окружения
                    env.FILE_CONTENT = fileContent // Переменная будет доступна во всех этапах
                    
                    // Вывод содержимого переменной окружения
                    echo "Содержимое переменной:\n${env.FILE_CONTENT}"
                }
            }
        }
    }
}

