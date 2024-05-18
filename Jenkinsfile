pipeline{
    agent any
    stages{
        stage("Test"){
            steps{
                sh '''
                       echo "Hello World"
                   '''
            }
        }
        stage("Build"){
            steps{
                sh '''
                      ## Get the project
                       
                       sudo apt update

                       docker build -t monyslim/pixer:latest .

                       docker run -d -p 80:80 monyslim/pixer:latest
                   
                   
                   
                   '''
            }
        }
    }
}