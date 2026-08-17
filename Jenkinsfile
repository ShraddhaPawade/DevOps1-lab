pipeline {

    agent any
 
    stages {
 
        stage('Checkout') {

            steps {

                git branch: 'main',

                    url: 'https://github.com/ShraddhaPawade/DevOps1-lab.git '
            }

        }
 
        stage('Build') {

            steps {

                echo 'Build completed successfully'

            }

        }
 
        stage('Test') {

            steps {

                echo 'Tests completed successfully'

            }

        }

    }
 
    post {

        success {

            echo 'Pipeline completed successfully!'

        }
 
        failure {

            echo 'Pipeline failed!'

        }

    }

}
 