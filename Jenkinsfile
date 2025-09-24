pipeline{
    agent any
    environment{
        ENV_VAR = "Hello from env"
    }
    tools{
        maven 'Maven 3.9.9'
        //java 'JDK-17'
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
        stage('Deploy'){
            steps{
                when{
                    branch 'master'
                    echo "can't deploy due to racism"
                }
            }
        }
    }
    post{
        always{
            echo 'WE FINISHED THE PIPELINE!'
        }
    }
}
