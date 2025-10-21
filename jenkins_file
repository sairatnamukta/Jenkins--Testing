pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Pull your code from Git
                git branch: 'main', url: 'https://github.com/sairatnamukta/Jenkins--Testing.git'
            }
        }

        stage('Run Script') {
            steps {
                echo 'Running test.py...'
                sh 'python3 Jenkins_Test_file_2.py'
                sh 'python3 Jenkins_Test_file.py'
            }
        }
    }

    post {
        always {
            echo 'Pipeline completed!'
        }
    }
}