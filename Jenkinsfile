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
                echo 'Building..'
				sh 'mvn package'
            }
        }
    }
}