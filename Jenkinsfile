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
             
           
            }
        }
    
}
