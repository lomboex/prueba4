pipeline {
    agent any

    stages {
        stage('Clonar Repo') {
            steps {
                git 'https://github.com/lomboex/prueba4.git'
            }
        }

        stage('Construir Imagen Docker') {
            steps {
                sh 'docker build -t mi-app:latest .'
            }
        }

        stage('Ejecutar Imagen Docker') {
            steps {
                sh 'docker run --rm mi-app:latest'
            }
        }
    }
}

