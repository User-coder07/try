pipeline {
    agent any  // Runs on any available Windows agent

    stages {
        stage('Checkout Code') {
            steps {
                // Clone your GitHub repository
                git branch: 'main' , url:'https://github.com/User-coder07/try.git'
            }
        }

      

        stage('Compile Java Code') {
            steps {
                    // Navigate to the directory where the Java file is located (if applicable)
                    bat 'javac Addition.java'
                }
            }
        

        stage('Run Java Program') {
            steps {
                    // Execute the Java program with input (Example: Finding primes between 10 and 50)
                    bat 'java Addition'
            }      
            
        }

     
    }
}
