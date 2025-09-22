pipeline{
    agent any
    stages{
        stage('First Build'){
            steps{
                sh '''
                    echo "Hello from Git!"
                '''
            }
        }
    }
    post{
        always{
            echo 'WE FINISHED THE PIPELINE!'
        }
    }
}