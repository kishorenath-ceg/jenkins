pipeline {
    agent any

    triggers {
        pollSCM('* * * * *')
    }

    stages {

        stage('Build') {
            steps {
                bat 'javac Hello.java'
            }
        }

        stage('Run') {
            steps {
                bat 'java Hello'
            }
        }
    }
}
