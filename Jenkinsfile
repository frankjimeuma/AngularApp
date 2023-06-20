pipeline {
    agent any

    stages {
        
        stage('Instalar dependencias') {
            steps {
                sh 'npm install'
            }
        }
        
      
        stage('Compilacion del APP') {
            steps {
                sh 'npm run build'
            }
        }

        stage('Mostrar Archivos') {
            
            steps {
                sh 'ls -la'
            }
        }
        //Despliegue
        stage('Despliegue de la Aplicacion') {
            steps {
                sh 'cp dist/democlase06/* /tmp/deploy'
            }
        }
    }
}