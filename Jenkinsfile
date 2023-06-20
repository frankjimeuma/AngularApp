pipeline {
    agent any

    stages {
        
        stage('Descargar Codigitos') {
            steps {
                sh 'npm install'
            }
        }
        
      
        stage('Despliegue en Ambiente de desarrollitos!!!s!') {
            steps {
                sh 'npm run build'
            }
        }

        stage('Mensaje final') {
            when {branch 'dev'}
            steps {
                echo 'Todo bien!'
            }
        }
    }
}