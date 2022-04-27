pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'nodejs' 
    }
   
    stages{
        stage('Compile'){
            steps{
                echo 'this is the Compile job'
                sh 'npm install'
            }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                sh 'npm test'
            }
        }
        stage('package'){
            steps{
                echo 'this is the package job'
                sh 'npm run package'
            }
        }
    }
    
    post{
        always{
            echo 'this is my dojo b13 pipeline has completed...'
        }
        
    }
    
}
