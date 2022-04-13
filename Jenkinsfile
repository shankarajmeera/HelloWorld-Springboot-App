pipeline{
    agent any
    stages{
        stage('Git clone'){
            steps{
                git 'https://github.com/shankarajmeera/HelloWorld-Springboot-App.git'
            }
        }
        
        stage('maven build'){
            steps{
                bat 'mvn package'
            }
        }
        stage('Create Dockerimage'){
            steps{
                bat 'docker build -t thetips4you/springboot:latest .'
            }
        }
        
    }
}
