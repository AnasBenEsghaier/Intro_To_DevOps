pipeline {
    agent any
	
    tools {
	maven 'M2_HOME'
    }
    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    credentialsId: 'Github_Token',
                    url: 'https://github.com/AnasBenEsghaier/Intro_To_DevOps.git'
            }
        }
	stage('build & package') {
		steps { 
			sh 'mvn clean package -DskipTests'
		}
	}    
    }
}
