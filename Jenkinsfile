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
//                 sh "chmod u+x Add.py"
                sh "/usr/bin/python3 Add.py"
            }
        }
        stage('Build Code 2') {
            steps {
//                 sh "chmod u+x Factorial.py"
                sh "/usr/bin/python3 Factorial.py"
            }
        }
        stage('Test Code') {
            steps {
//                 sh "chmod u+x Test.py"
                sh "/usr/bin/python3 Test.py"
            }
        }
    } 
}
