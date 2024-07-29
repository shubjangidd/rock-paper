pipeline {
    agent any
        stage('Build') {
            steps {
                sh 'mvn package'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
                sh 'cd target'
                sh 'mv roshambo.war pipeline.war'
            }
        }        
        stage('Deploy') {
            steps {
               deploy adapters: [tomcat9(credentialsId: 'fbedcda7-ed83-4521-b672-b87875ed4ff9', path: '', url: 'http://13.69.144.11:8090/')], contextPath: null, war: '**/*.war'
            }
        }       
    }
}