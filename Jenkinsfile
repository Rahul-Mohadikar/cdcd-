pipeline {
    agent any 
    
    tools{
        jdk 'java'
        maven 'maven'
    }
    
     stages{
        
        stage("Git Checkout"){
            steps{
                git branch: 'main', changelog: false, poll: false, url: 'https://github.com/Rahul-Mohadikar/cdcd-.git'
            }
        }
        
        stage("Compile"){
            steps{
                sh "mvn clean compile"
            }
        }
        
     }
}

