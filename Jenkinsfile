pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
               git branch: 'main', url: 'https://github.com/shravanim367-lab/Jenkins-Demo.git'

            }
        }

        stage('Build') {
            steps {
                bat 'python app.py'
            }
        }

        stage('Test') {
            steps {
                bat 'python test.py'
            }
        }
    }
}
