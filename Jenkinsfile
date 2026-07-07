pipeline{
    agent any
    stages{
        stage(hello){
            steps{
                echo "hello"
            }
        }

        stage(npm){
            steps{
                npm --version
                npm start
            }
        }
        }
    }
}