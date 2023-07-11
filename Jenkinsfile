pipeline {
    agent{
         docker{
            image 'node:6-alpine'
            args '-p 3000:3000'
    }
    } 
    environment {
        CI='true'
    }

    stages {
        stage('Build') {
            script{
            steps {
                npm i
                npm run build
            }
            }
        }
        stage('Test') {
            script{
            steps {
                npm i
                npm run test
            }
            }
            
        }
       
    }
}