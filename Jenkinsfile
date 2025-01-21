pipeline {
    agent any

    triggers {
        githubPush() //Escuchar cuando ocurra un evento push
    }
    
    stages {
        stage('Clonar repositorio..') {
            steps {
                echo 'Iniciando el clonado del repositorio...'
                git branch: 'develop', url: 'https://github.com/fercdev/jenkins-pipeline-txt.git'
            }
        }

        stage('Listar estructura de proyecto..') {
            steps {
                echo 'Listar la estructura de mi repositorio...'
                sh 'ls -R'
            }
        }
    }
}