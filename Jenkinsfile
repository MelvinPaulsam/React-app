pipeline {
    agent any
    environment {
        CI='true'
    }

    stages {
        stage('Build') {
            
            steps {
                script{
                npm i
                npm run build
            }
            }
        }
        stage('Test') {
            
            steps {
                script{
                npm i
                npm run test
            }
            }
            
        }
       
    }
}