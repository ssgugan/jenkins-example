pipeline{
    agent any
    environment {
        PATH = "$PATH:/opt/apache-maven-3.8.5/bin"
    }
    stages{
       stage('GetCode'){
            steps{
                git 'https://github.com/selvigugan/hello-world.git'
            }
         }        
       stage('Build'){
            steps{
                sh 'mvn clean package'
            }
         }
    }
}
