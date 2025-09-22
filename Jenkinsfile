pipeline{
    agent any
    environment{
        ENV_VAR = "Hello from env"
    }
    stages{
        stage('First Build'){
            steps{
                sh '''
                    echo "Hello from Git!"
                    
                '''
                echo "the ENV is: ${ENV_VAR}"
            }
        }
    }
    post{
        always{
            echo 'WE FINISHED THE PIPELINE!'
        }
    }
}