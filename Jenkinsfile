pipeline {
    agent any 
    
    tools{
        jdk 'java'
        maven 'maven'
    }
    
     stages{
        
        stage("Git Checkout"){
            steps{
                scm checkout
            }
        }
        
        stage("Compile"){
            steps{
                sh "mvn clean compile"
            }
        }
        
     }
}

