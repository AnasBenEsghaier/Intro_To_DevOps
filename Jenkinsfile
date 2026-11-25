pipeline {
    agent any
	
    tools {
	jdk 'JAVA_HOME'
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
			cd Backend 
			sh 'mvn clean package -DskipTests'
		}
	}    
    }
}
