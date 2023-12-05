pipeline {

    agent any

    stages {

        stage('Echoing') {

            steps {
                sh '''
                pwd
                echo "Hi there"
                echo "My name is"
                echo "Michael Yarborough"
                '''

                //

            }

        }

        stage('Running Script') {

            steps {

                // This runs a script
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