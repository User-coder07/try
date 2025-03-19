pipeline {
    agent any
    stages {
        stage('Clone repository') {
            steps {
                 git branch: 'main' , url:'https://github.com/User-coder07/try.git'
            }
        }    
        stage('Compile Java Code') {
            steps {
                    bat 'javac Addition.java'
                }
            }       
        stage('Run Java Program') {
            steps {
                    bat 'java Addition'
            }   
        }

     }
}
