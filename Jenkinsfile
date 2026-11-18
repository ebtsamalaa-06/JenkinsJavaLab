pipeline {
    agent any

    stages {
        stage('Check Java') {
            steps {
                bat 'where java'
                bat 'where javac'
                bat 'java -version'
                bat 'javac -version'
            }
        }

        stage('Compile') {
            steps {
                echo 'Compiling...'
                bat 'javac HelloWorld.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Running...'
                bat 'java HelloWorld'
            }
        }
    }
}
