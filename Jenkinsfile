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

        stage('Despliegue de aplicacion') {
            steps {
                sh 'cp /dist/AngularApp-Frank/* /tmp/deploy'
            }
        }
    }
}