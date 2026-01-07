pipeline {
    agent any

    stages {}

        stages {
            stage('clean workspace') {
                steps {
                    deleteDir()
                }
         }
         stage('Clone Git Repo') {
                steps {
                    sh 'git clone https://github.com/codingsandy/jenkins-docker-demo.git .'
                }
         stage( 'Build Docker Image') {
                steps {
                   sh 'docker build -t sandy-ngnix .' 
                }
            }
         }

}
