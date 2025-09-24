pipeline{
    agent any
    environment{
        ENV_VAR = "Hello from env"
    }
    tools{
        maven 'Maven-3.8.6'
        java 'JDK-17'
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