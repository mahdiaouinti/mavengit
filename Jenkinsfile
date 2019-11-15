pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                sh label: '', script: 'mvn install '
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
