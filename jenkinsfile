pipeline {
    agent any 
    stages {
        stage('clone repository & compile') { 
            steps {
                sh " mvn clean compile"
            }
        }
        stage('Test') { 
            steps {
                sh " mvn test " 
            }
        }
        stage('Deploy') { 
            steps {
                sh " mvn package " 
            }
        }
    }
}
