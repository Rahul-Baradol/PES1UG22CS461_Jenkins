pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o PES1UG22CS461-1 main/hello.cpp'

                }
            }
        }
        
        stage('Test') {
            steps {
                script {
                    sh './PES1UG22CS461-1'
			intentional error
                }
            }
        }
        
        stage('Deploy') {
            steps {
                script {
            		echo 'Deploying...'
		 }
            }
        }
    }
    
    post {
        failure {
            echo 'pipeline failed'
        }
    }
}
