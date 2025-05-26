pipeline{
    agent{
        label "agent-0"
    }
   
    stages{
        stage("build Docker image"){
            steps{
                sh "docker build -t mohamedomaraa/data-iti:v${BUILD_NUMBER} ."
            }
        }
        stage("Push Docker image"){
            steps{
                sh "docker push mohamedomaraa/data-iti:v${BUILD_NUMBER}"
            }
        }
    }
}