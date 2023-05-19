pipeline {
    agent any
  stages {    
    
    stage('Checkout external proj') {
        steps {
            git branch: 'master',
                credentialsId: '922aa409-e2fd-4bc9-bb8d-47204bfc9cd7',
                url: 'https://github.com/dburcombe/using_groovy.git'

            
        }
    }
  
        stage('Hello') {
            steps {
                sh 'python3 operations.py'
            }
        }
    }
}

