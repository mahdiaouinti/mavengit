pipeline {
    agent any

    stages {
        stage("mvn build") {
            steps {
               steps {
                echo 'Building..'
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
