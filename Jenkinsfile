pipeline {
    agent {
        label "master"
    }
    tools {
        maven 'Maven'
        jdk 'JAVA'
    }
    stages {
        stage ('Initialize') {
            steps {
           
                    echo "PATH = %PATH%"
                    echo "M2_HOME = %M2_HOME%"
               
            }
        }

        stage ('Build') {
            steps {
                    sh 'mvn clean compile'
            }
             
               stage ('Compile stage') {
                    steps {
                          
                             sh 'mvn clean compile'
                             }
                       
                  }

               stage ('Testing stage') {
                    steps {
                           
                             sh 'mvn test'
                             }
                       
                  }

               stage ('Deployment stage') {
                    steps {
                           
                             sh 'mvn deploy'
                             }
                        
                  }
           
            }
        }
    
}
