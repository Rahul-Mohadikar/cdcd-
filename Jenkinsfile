pipeline {
    agent any 
    
    tools{
        jdk 'java'
        maven 'maven'
    }
    
     stages{
        
        stage("Git Checkout"){
            steps{
               checkout scm
            }
        }
        
        stage("Compile"){
            steps{
                sh "mvn clean compile"
            }
        }
        
     }
}

