pipeline {
    agent any

    stages {
        
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        
        
             stage('java') {
            steps {
                git branch: 'main', url: 'https://github.com/abhinait29/abhi-javaproject.git'
                bat '''javac App.java
            java App.java'''
            }   
            }
            
            
            stage('maven') {
            steps {
                git 'https://github.com/abhinait29/abhi-mvnproject1.git'
                bat 'mvn clean test'
            }
            }
        
    }
}
