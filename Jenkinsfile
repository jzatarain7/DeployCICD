pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'dev', url: 'https://github.com/jzatarain7/DeployCICD.git'
            }
        }

        stage('Build Docker') {
            steps {
                sh 'docker build -t node-api -f CICD/Dockerfile .'
            }
        }
        echo "🚀 Hasta aqui todo bien. ${env.BRANCH_NAME}" 

        /*stage('Copy files to WSL folder') {
            steps {
                sh '''
                rm -rf /mnt/c/Users/tuusuario/APINodeExpress/*
                cp -r * /mnt/c/Users/tuusuario/APINodeExpress/
                '''
            }
        }

        stage('Run Docker Compose in WSL') {
            steps {
                sh '''
                cd /mnt/c/Users/tuusuario/APINodeExpress/CICD
                docker-compose up -d --build
                '''
            }
        }*/
    }
}
