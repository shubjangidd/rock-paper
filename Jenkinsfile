pipeline {
    agent any

    stages {
        stage('clone') {
            steps {
                
            }
        }
        stage('Build') {
            steps {
                // sh 'mvn package'
            }
        }
        stage('Test') {
            steps {
                // sh 'mvn test'
            }
        }        
        stage('Deploy') {
            steps {
                // sshagent(credentials: ['tomcat']) {
                //     sh 'scp -oStrictHostKeyChecking=no target/*.war USERNAME@IPADDRESS:TYPE_PATH'
                
                }
            }
        }       
    }
}