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
                echo 't1....'
                git 'https://github.com/mahdiaouinti/mavengit'
            }
        }
        stage('Test') {
            steps {
                echo 't2....'
                sh label: '', script: 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 't3....'
                echo 'Deploying....'
            }
        }
    }
}
