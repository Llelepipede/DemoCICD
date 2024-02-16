pipeline {
    agent any
    tools {maven "Maven"}

    stages {
        stage('Checkout') {
            steps{
                git branch: 'main', url: 'https://github.com/Llelepipede/JenkinsTest'
            }
        }
        stage('javadoc') {
            steps{
                sh 'mvn javadoc:javadoc'
            }
        }
        stage('Build') {
            steps{
                sh 'mvn compile'
            }
        }
    }
}