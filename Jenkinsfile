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
                sh "chmod u+x b.c"
                sh "gcc b.c -o b"
            }
        }
        stage('Execute a.c') {
            steps {
                sh "chmod u+x b"
                sh "./b"
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
