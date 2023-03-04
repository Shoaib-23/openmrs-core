# Create Declarative Pipeline For OpenMRS:
------------------------------------------

---
pipeline {
    agent { label 'OPENMRS' }
    stages {
        stage('git clone') {
            steps {
                git url: 'https://github.com/Shoaib-23/openmrs-core.git',
                    branch: 'declarative'
            }
        }   
        stage('build') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
---