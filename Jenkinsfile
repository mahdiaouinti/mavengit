pipeline {
    agent any
   
    stages {
        stage("mvn build") {
            steps {
               
                echo 'Building..'
                   script {
                    // If you are using Windows then you should use "bat" step
                    // Since unit testing is out of the scope we skip them
                    bat 'mvn install'
                }
            
            }
        }
        stage('checkout') {
            steps {
                git 'https://github.com/mahdiaouinti/mavengit'
            }
        }
        stage('Test') {
            steps {
                bat label: '', script: 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                 bat label: '', script: 'install deploye'
            }
        }
    
    }
}
