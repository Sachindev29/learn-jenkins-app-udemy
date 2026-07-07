pipeline{
    agent any
    stages{
        stage('hello'){
            steps{
                echo "hello"
            }
        }

        stage('npm'){
            steps{
               sh 'npm --version'
               sh 'npm start'
            }
        }
        }
    }