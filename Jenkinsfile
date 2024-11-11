pipeline{
    agent any
    tools{
        jdk 'Java 11'
        maven 'maven'
    }
    stages{
        stage('git checkout'){
            steps{
                git branch: 'main', url: 'https://github.com/TushR007/test-devops.git'
            }
        }
        stage('compile'){
            steps{
                sh 'mvn compile'
            }
        }
        stage('build'){
            steps{
                sh 'mvn package'
            }
        }
    }
}