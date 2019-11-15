pipeline {
    agent any

    stages {
        
        stage('build') {
            steps {
                sh label: '', script: 'mvn install '
            }
        }
        
        
        stage('checkout') {
            steps {
                git 'https://github.com/mahdiaouinti/mavengit'
            }
        }
        stage('Test') {
            steps {
                sh label: '', script: 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
