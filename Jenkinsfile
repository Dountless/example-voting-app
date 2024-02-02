pipeline{
    agent{
        label "my-deployment"
    }
    stages{
        stage("SetUp"){
            steps{
                sh 'echo "hello"'
            }

        }
        stage("Build Image"){
            steps{
           echo 'Start building the project docker image for production'
          script {
             testImage = docker.build("amankumar19/myvotingapp:latest", "-f ./vote/Dockerfile .")
            //  testImage.push()
            }

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
