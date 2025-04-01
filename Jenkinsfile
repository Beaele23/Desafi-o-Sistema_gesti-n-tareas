pipeline {
    agent any
    stages {
        stage('Clonar repositorio') {
            steps {
                git 'https://github.com/tu_usuario/nombre_repositorio.git'
            }
        }
        stage('Instalar dependencias') {
            steps {
                sh 'npm install'
            }
        }
        stage('Ejecutar pruebas') {
            steps {
                sh 'npm test'
            }
        }
        stage('Construir imagen Docker') {
            steps {
                sh 'docker build -t gestion-tareas-api .'
            }
        }
    }
}
