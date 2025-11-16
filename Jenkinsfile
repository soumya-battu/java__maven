pipeline {
    agent any

    tools {
        maven 'Maven 3.9.11'
    }

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/soumya-battu/java__maven.git'
            }
        }

        stage('Build with Maven') {
            steps {
                bat "mvn clean install"
            }
        }

        stage('Archive WAR') {
            steps {
                archiveArtifacts artifacts: 'target/*.war', fingerprint: true
            }
        }
    }
}
