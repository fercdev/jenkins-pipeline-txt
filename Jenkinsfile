pipeline {
    agent any

    triggers {
        githubPush() //Escuchar cuando ocurra un evento push
    }
    
    stages {
        stage('Clonar repositorio...') {
            steps {
                echo 'Clonando mi repositorio'
                git branch: 'develop', url 'https://github.com/fercdev/jenkins-pipeline-txt.git'
            }
        }

        stage('Listar estructura...') {
            steps {
                echo 'Listando todas las carpetas y archivos...'
                sh 'ls -la'
            }
        }
    }
}