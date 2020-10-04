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
                sh 'git pull origin main --allow-unrelated-histories'
                sh 'git merge dev'
                sh 'git push origin main'
                
            }
        }
    }
}
