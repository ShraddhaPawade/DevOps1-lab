pipeline { 

 

    agent any 

 

    stages { 

 

        stage('Checkout') { 

            steps { 

                git 'https://github.com/ShraddhaPawade/DevOps1-lab.git
' 

            } 

        } 

 

        stage('Install Dependencies') { 

            steps { 

                bat 'pip install -r requirements.txt' 

            } 

        } 

 

        stage('Build') { 

            steps { 

                bat 'python app.py' 

            } 

        } 

 

        stage('Test') { 

            steps { 

                bat 'pytest' 

            } 

        } 

    } 

 

    post { 

        always { 

            junit '**/test-results.xml' 

        } 

    } 

}