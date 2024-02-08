pipeline {
    agent any
    tools {maven "Maven"}

    stages {
        stage('Checkout') {
            steps{
                git branch: 'main', url: 'https://github.com/Llelepipede/JenkinsTest'
            }
        }
        stage('Build') {
            steps{
                bat 'mvn compile'
            }
        }
    }