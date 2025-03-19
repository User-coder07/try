pipeline {
    agent any
    environment {
        JAVA_HOME = "C:/Program Files/Java/jdk-21"  // Replace with your JDK path
        PATH = "${JAVA_HOME}\\bin;${env.PATH}"
    }
    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main' , url: 'https://github.com/User-coder07/try.git'
            }
        }
        stage('Compile Java Code') {
            steps {
                    bat '"%JAVA_HOME%\\bin\\javac" Addition.java'
                }
            
        }
        stage('Run Java Program') {
            steps {
                
                    bat '"%JAVA_HOME%\\bin\\java" Addition'
                
            }
        }
    }
}
