pipeline {
    tools {
    maven "apache-maven-3.6.3"
    jdk "default"
    }
    agent {
        label 'jnlp'
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
