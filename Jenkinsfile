pipeline {
    agent any

    stages {
        stage('clone') {
            steps {
                echo 'Hello world!'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn package'
            }
        }
        stage('Test') {
            steps {
                 echo 'Hello world!'
                // sh 'mvn test'
            }
        }        
        stage('Deploy') {
            steps {
             echo 'Hello world!'
                // sshagent(credentials: ['tomcat']) {
                //     sh 'scp -oStrictHostKeyChecking=no target/*.war USERNAME@IPADDRESS:TYPE_PATH'
                // }
            }
        }       
    }
}