pipeline {
    agent any

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

