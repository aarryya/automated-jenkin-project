pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                bat '"C:\\Users\\Aarya\\AppData\\Local\\Programs\\Python\\Python314\\python.exe" -m pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                bat '"C:\\Users\\Aarya\\AppData\\Local\\Programs\\Python\\Python314\\python.exe" -m pytest'
            }
        }

        stage('Run Application') {
            steps {
                bat '"C:\\Users\\Aarya\\AppData\\Local\\Programs\\Python\\Python314\\python.exe" app.py'
            }
        }
    }
}