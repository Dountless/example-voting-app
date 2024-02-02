pipeline{
    agent any
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
            //  testImage = docker.build("amankumar19/myvotingapp:latest", "-f ./Dockerfile .")
            //  testImage.push()
            echo "buildsuccessfully "
            }

            }

        }
        stage("deploy to deployment-server"){
            agent{
                  label "my-deployment"
                }
            steps{
                // sh "docker build -t amankumar19/voting-app:latest . "
                sh '''
                    docker container run -d --name myweb -p 80:80 nginx 
                '''
            }

        }
    }
}
