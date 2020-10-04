pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('merge') {
            steps {
                sh 'git pull origin dev'
                sh 'git checkout main'
                sh 'git pull origin main'
                sh 'git merge dev'
                sh 'git push origin main'
                
            }
        }
    }
}
