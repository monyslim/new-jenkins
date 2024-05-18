pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh '''
                    echo "Hello World"
                   '''
            }
            
        }
    }
    stages{
        steps("Build the image"){
            steps{
                sh '''
                       ## Get the project
                       
                       sudo apt update

                       cd /home/david/new-pixer

                       docker build -t monyslim/pixer:latest .

                       docker run -d -p 80:80 monyslim/pixer:latest

                       
                   
                   
                   '''
            }
        }
    }
}