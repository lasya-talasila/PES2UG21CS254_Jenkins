pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                script {
                    // Compile .cpp file using shell script
                    sh 'g++ -o my_program PES2UG2154.cpp'
                }
            }
        }
        
        stage('Test') {
            steps {
                script {
                    // Print output of .cpp file using shell script
                    sh './my_program'
                }
            }
        }
        
        stage('Deploy') {
            steps {
                script {
                    // Deploy your application if needed
                    // This stage is a placeholder and can be customized as per your requirements
                    echo 'Deployment step can be added here'
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
