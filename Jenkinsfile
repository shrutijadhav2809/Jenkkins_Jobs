pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/shrutijadhav2809/Jenkkins_Jobs.git'
            }
        }

        stage('Compile Java Program') {
            steps {
                bat 'javac EvenOdd.java'
            }
        }

        stage('Run Java Program') {
            steps {
                bat 'echo 5 | java EvenOdd'
            }
        }
    }
}
