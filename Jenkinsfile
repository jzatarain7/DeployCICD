pipeline {
    agent any

    stages {
        stage('Muerstra variables de enotnro') {
            steps {
                echo "Hola manuel, eres mi hijo no l oolvides y ando deployando."
                sh 'printenv' // Muestra todas las variables de entorno en Linux
                echo "PATH: ${env.PATH}"
                echo "BRANCH_NAME: ${env.BRANCH_NAME}"
                echo "BUILD_NUMBER: ${env.BUILD_NUMBER}"
                echo "JOB_NAME: ${env.JOB_NAME}"
                echo "WORKSPACE: ${env.WORKSPACE}"
                echo "Fin de tercera prueba" 
            }
        }
    }
}