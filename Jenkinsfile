pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                sh "rm -rf *"
                sh "git clone https://github.com/saknouche/jenkins-helloworld"
            }
        }
        stage('Build') {
            steps {
                  sh "cd jenkins-helloworld && javac Main.java"
            }
        }
         stage('Run') {
            steps {
                  sh "cd jenkins-helloworld && java Main"
            }
        }
        
    }
}