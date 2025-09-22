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
                echo "ENV is: ${ENV_VAR}"
                echo "Job Name is: ${JOB_NAME}"
                

            }
        }
    }
    post{
        always{
            echo 'WE FINISHED THE PIPELINE!'
        }
    }
}