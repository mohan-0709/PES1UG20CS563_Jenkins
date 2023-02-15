pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'g++ -c PES1UG20CS563.cpp'
                sh 'g++ -o PES1UG20CS563 PES1UG20CS563.cpp'
                echo 'build stage is successfull'
            }
        }
        stage('Test'){
            steps{
                sh './PES1UG20CS563'
                echo 'Test stage is successfull'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deployement is successfuLLLL'
            }
        }
    }
    post{
        failure{
            echo 'Pipeline Failed'
        }
    }
}
