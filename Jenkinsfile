pipeline {
    agent any

    stages {
        stage('clone') {
            steps {
                git branch: 'cse',
                    url: 'https://github.com/harshith301/devopslabdemo.git'
            }
        }

        stage('build') {
            steps {
                sh 'javac Hello.java'
            }
        }

        stage('run') {
            steps {
                sh 'java Hello'
            }
        }
    }
}
