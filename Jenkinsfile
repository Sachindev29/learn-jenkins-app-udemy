pipeline{
    agent any
    stages{
        stage('build'){
            agent{
                docker {
                    image 'node:18-alpine'
                    reuseNode true
                }
            }
            steps{
                sh '''
                ls -la
                npm --version
                npm ci
                npm test
                npm run build
                ls -la
                '''
            }
        }
        stage ('test'){
            steps{
                sh 'npm test'
                echo "test completed"
            }
        }

        }
    }