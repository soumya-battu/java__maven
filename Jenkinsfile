
    tools {            steps {
                git branch: 'main', url: 'https://github.com/soumya-battu/java__maven.git'
            }
        }

        stage('Build with Maven') {
            steps {
          
        }

        stage('Archive WAR') {
            steps {
                archiveArtifacts artifacts: 'target/*.jar', fingerprint: true
            }
        }
    }
}
