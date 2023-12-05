pipeline {

    agent any

    stages {

        stage('Echoing') {

            steps {
                sh '''
                echo "Hi thre"
                echo "Groovy Baby"
                echo "inside shell block"
                '''
          
            }

        }

        stage('Running Script') {

            steps {
                sh '''
                sh ./run.sh
                '''               

            }

        }
    }
    post {
        always {
            archiveArtifacts '*.zip'
        }
    }
}


