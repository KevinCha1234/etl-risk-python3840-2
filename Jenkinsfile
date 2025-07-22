pipeline {
    agent any

    stages {
        stage('Clonar repositorio') {
            steps {
                git branch: 'develop', url: 'https://github.com/KevinCha1234/etl-risk-python3840-2.git'
            }
        }

        stage('Ejecutar ETL') {
            steps {
                sh 'python transform.py'
            }
        }
    }
}
