pipeline{
    agent any
    stages{
        stage('checkout the code from github'){
            steps{
                 git url: 'https://github.com/sunilkumar15874/Banking-java-project/'
                 echo 'github url checkout'
            }
        }
        stage('codecompile with sunil'){
            steps{
                echo 'starting compiling'
                sh 'mvn compile'
            }
        }
        stage('codetesting with sunil'){
            steps{
                sh 'mvn test'
            }
        }
        stage('qa with sunil'){
            steps{
                sh 'mvn checkstyle:checkstyle'
            }
        }
    }    
}
