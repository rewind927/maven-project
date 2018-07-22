pipeline {
    agent any
    stages{
        stage('Build'){
            steps {
                echo 'start Build'
            }
            post {
                success {
                    echo 'Now Archiving...'
                }
            }
        }
    }
}
