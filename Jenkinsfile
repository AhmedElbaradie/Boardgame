pipeline {
    agent {
        label 'slave'
    }
    tools {
        jdk 'jdk 17'
        maven 'maven 3'
    }
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/AhmedElbaradie/Boardgame.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
