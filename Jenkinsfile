pipeline {
    agent any

    stages {
        stage('Clonar repositorio') {
            steps {
                git branch: 'develop', url: 'https://github.com/jcrodas88/etl-risk-python.git'
            }
        }

        stage('Ejecutar ETL') {
            steps {
                sh 'python lectura.py'
            }
        }
    }
}
