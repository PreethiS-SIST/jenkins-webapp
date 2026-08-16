pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building application successfully'
                sh 'mvn clean package'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying to Tomcat'
                sh 'cp target/*.war /opt/tomcat/apache-tomcat-10.1.57/webapps/'
            }
        }
    }
}
