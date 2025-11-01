pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building Project...'
                bat 'build.bat'   // runs your build.bat
            }
        }

        stage('Test') {
            steps {
                echo 'Running Tests...'
                bat 'test.bat'    // runs your test.bat
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying Application...'
                bat 'deploy.bat'  // runs your deploy.bat
            }
        }
    }
}
