pipeline {
    agent any

    stages {
        stage("mvn build") {
            steps {
               
                echo 'Building..'
                   script {
                    // If you are using Windows then you should use "bat" step
                    // Since unit testing is out of the scope we skip them
                    bat "mvn package -DskipTests=true"
                }
            
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
