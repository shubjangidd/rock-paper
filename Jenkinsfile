pipeline {
    agent any

    stages {
        stage('clone') {
            steps {
                // git credentialsId: 'github', url: 'https://github.com/aftab70/maven.git'
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