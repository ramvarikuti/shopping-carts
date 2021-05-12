pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
   Tools{
maven ‘maven’        

    }
   

    stages{
        stage('build'){
            steps{
                echo 'this is the build job'
                sh 'mvn compile'
            }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                sh 'mvn test'
                //sleep 9
            }
        }
        stage('package'){
            steps{
                echo 'this is the package job'
                sh ‘mvn package'
                //sleep 7
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}

