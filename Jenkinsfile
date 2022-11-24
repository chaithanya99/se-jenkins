pipeline { 
    agent any
    stages {
        stage('Clone Git') {
            steps {
                git 'https://github.com/pavanthanay/se-jenkins.git'
            }
        }
        stage('Build Code 1') {
            steps {
                sh "chmod u+x Add.py"
                sh "./Add.py"
            }
        }
        stage('Build Code 2') {
            steps {
                sh "chmod u+x Factorial.py"
                sh "./Factorial.py"
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
