pipeline { 
    agent any
    stages {
        stage('Clone Git') {
            steps {
                git 'https://github.com/arnabnath180/Jenkins_Pipeline.git'
            }
        }
        stage('Build a.c') {
            steps {
                sh "chmod u+x a.c"
                sh "gcc a.c"
            }
        }
        stage('Execute a.c') {
            steps {
                sh "chmod u+x a.out"
                sh "./a.out"
            }
        }
        stage('Build Code') {
            steps {
                sh "chmod u+x Prog1.py"
                sh "./Prog1.py"
            }
        }
     stage('Test Code') {
            steps {
                sh "chmod u+x Test.py"
                sh "./Test.py"
            }
        }
    } 
}
