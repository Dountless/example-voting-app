pipeline{
    agent{
        label "my-deployment"
    }
    stages{
        stage("Build Image"){
            steps{
                sh 'touch helloooooo'
            }

        }
        stage("push to dockerhub"){
            steps{
                // sh "docker build -t amankumar19/voting-app:latest . "
                sh 'echo "hello"'
            }

        }
        stage("deploy to deployment-server"){
            steps{
                // sh "docker build -t amankumar19/voting-app:latest . "
                sh 'echo "hello"'
            }

        }
    }
}
