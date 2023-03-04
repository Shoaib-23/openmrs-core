pipeline {
    agent { label 'OPENMRS' }
	tools { maven "MAVEN-3.9.0" }
    stages {
        stage('git clone') {
            steps {
                git url: 'https://github.com/Shoaib-23/openmrs-core.git',
                    branch: 'declarative'
            }
        }   
        stage('build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
