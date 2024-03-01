pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
            git 'https://github.com/Nivedhidha2001/SPBootJenkins.git'
            sh'./mvnw compile'
                echo 'Maven build successfully !!'
            }
        }
        stage('Test') {
            steps {
            sh'./mvnw test'
          echo 'TestCases Executed successfully !!'
            }
        }
        stage('Package') {
            steps {
            sh'./mvnw package'
                echo 'Application deployed successfully !!'
            }
        }
    }
}