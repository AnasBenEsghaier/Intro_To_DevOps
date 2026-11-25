pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    credentialsId: 'Github_Token',
                    url: 'https://github.com/AnasBenEsghaier/Intro_To_DevOps.git'
            }
        }
    }
}
