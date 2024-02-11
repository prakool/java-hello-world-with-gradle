pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                script {
                    
                    echo 'Checkout1'
                }
            }
        }

        stage('Build') {
            steps {
                script {
                   
                   echo 'Build Started'
                    bat './gradlew.bat clean build'
                    echo 'Build Ended'
                    
                }
            }
        }

        stage('Test') {
            steps {
                script {
                   
                   echo 'Test1'
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                  
                   echo 'Deploy1'
                }
            }
        }
    }

    post {
        success {
            echo 'Pipeline succeeded! Send notifications, etc.'
        }
        failure {
            echo 'Pipeline failed! Send notifications, etc.'
        }
    }
}
