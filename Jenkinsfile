pipeline{
    agent any
    stages{
        stage('checkout the code from github'){
            steps{
                 git url: 'https://github.com/Mallaiah0938/Mallaiah-banking-project'
                 echo 'github url checkout'
            }
        }
        stage('codecompile with mallaiah'){
            steps{
                echo 'starting compiling'
                sh 'mvn compile'
            }
        }
        stage('codetesting with mallaiah'){
            steps{
                sh 'mvn test'
            }
        }
        stage('qa with mallaiah'){
            steps{
                sh 'mvn checkstyle:checkstyle'
            }
        }
        stage('package with mallaiah'){
            steps{
                sh 'mvn package'
            }
        } 
    }
}

    
