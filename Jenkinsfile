pipeline {
    agent any

    stages {
        stage("mvn build") {
            steps {
               
                echo 'Building..'
                   sh label: '', script: 'mvn install'
            
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
