pipeline {
    agent any

    stages {
        stage('SCM') {
            steps {
                echo 'Cloning source code..'
				checkout scm
            }
        }
		stage('Build') {
            steps {
                echo 'Building java application..'
				sh 'mvn -f InformationCentre/pom.xml package'
            }
        }
    }
}