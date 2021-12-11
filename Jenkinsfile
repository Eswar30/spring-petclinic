pipeline {
    agent {
	         label 'Build-server-1'
		}
    tools{
          maven 'Maven'
		      jdk 'Java'
		}
    stages {
        stage('validate') {
            steps {
                sh 'mvn validate'
            }
        }
		stage('compile') {
            steps {
                sh 'mvn compile'
            }
        }
		stage('test') {
            steps {
                sh 'mvn test'
            }
        }
		stage('package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
