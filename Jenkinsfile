pipeline {
    agent any
    stages{
        stage('Build'){
            steps {

            def mvn_version = 'M3'
            withEnv( ["/Users/rewind927/Documents/apache-maven-3.5.4/bin"] ) {
              sh 'mvn clean package'
            }
            }
            post {
                success {
                    echo 'Now Archiving...'
                    archiveArtifacts artifacts: '**/target/*.war'
                }
            }
        }
    }
}