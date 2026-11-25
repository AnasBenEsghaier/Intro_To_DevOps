pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    credentialsId: 'github-creds',
                    url: 'https://github.com/AnasBenEsghaier/Intro_To_DevOps.gitt'
            }
        }
    }
}
