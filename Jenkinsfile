pipeline{
        agent any
        stages{
             stage('install dependencies'){
                steps{
                    sh "bash install-dependencies.sh"
                }
            }
            stage('Deploy app'){
                steps{
                    sh "sudo docker-compose up -d --build"
                }
            }
        }    
}
