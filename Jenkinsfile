pipeline {
    agent any
    stages {
        stage('development') {
            when {
                branch 'development'
            }
            steps {
                sh 'cat git-branch.txt'
            }
        }
        stage('qa') {
            when {
                branch 'qa'
            }
            steps {
                sh 'cat git-branch.txt'
            }
        }
        stage('prod') {
            when {
                branch 'master'
            }
            steps {
                sh 'cat git-branch.txt'
            }
        }
    }
}