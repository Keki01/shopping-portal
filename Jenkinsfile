pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
   tools{
       nodejs'nodejs' 
    }
*/    

    stages{
        stage('one'){
            steps{
                echo 'this is the first job'
                sh 'npm install'
            }
        }
        stage('two'){
            steps{
                echo 'this is the second job'
                sh 'npm test'
            }
        }
        stage('three'){
            steps{
                echo 'this is the third job'
                sh 'npm run package'
            }
        }
    }
    
    post{
        always{
            echo 'this my dojo batch 13 nodejs  pipeline completed...'
        }
        
    }
    
}
