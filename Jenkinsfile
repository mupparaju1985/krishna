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
                sh 'git push origin main'
                sh 'git checkout master'
                sh 'git pull origin master'
                sh 'git merge main'
                sh 'git push origin master'
                
            }
        }
    }
}
