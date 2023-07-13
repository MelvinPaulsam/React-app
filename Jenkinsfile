pipeline {
    agent any
    

    stages {
        stage('init')
        {
            steps{
              
                    nodejs('Node'){
                        sh 'yarn install'
                    }
                
            }
        }
        stage('Build') {
            
            steps {
               
                
                nodejs('Node'){
                       sh  'yarn build'
                    }
            }
            
        }
        stage('Test') {
            
            steps {
             
                
                 nodejs('Node'){
                        sh 'yarn test'
                    }
            
            }
            
        }
       
    }
}