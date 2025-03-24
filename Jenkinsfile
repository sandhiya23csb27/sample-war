pipeline {
    agent any

    stages {
        stage('Checkout Source Code') {
            steps {
                git 'https://github.com/your-github-username/sample-war.git'
            }
        }

        stage('Build with Maven') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Deploy to Tomcat') {
            steps {
                sh 'cp target/*.war /opt/tomcat/webapps/sample.war'
            }
        }

        stage('Show Output') {
            steps {
                echo 'Deployment Successful - Sandhiya'
            }
        }
    }
}

