pipeline{
    agent any
    stages{
        stage('build'){
            agent{
                docker {
                    image 'node:18-alphine'
                    reuseNode true
                }
            }
            steps{
                sh '''
                ls -la
                npm --version
                npm ci
                npm run build
                ls -la
                '''
            }
        }

        }
    }