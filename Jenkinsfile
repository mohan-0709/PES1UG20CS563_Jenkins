pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'g++ -c main/hello.cpp'
                sh 'g++ -o PES1UG20CS563 main/hello.cpp'
                echo 'build stage is successful'
            }
        }
        stage('Test'){
            steps{
                sh './PES1UG20CS0563'
                echo 'test stage is successful'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deployment is Successful'
            }
        }
    }
    post{
        failure{
            echo 'Pipeline Failed'
        }
    }
