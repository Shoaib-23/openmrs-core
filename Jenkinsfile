node('OPENMRS') {
    stage('VCS') {
        git url: 'https://github.com/Shoaib-23/openmrs-core.git',
            branch: 'scripted'    
    }
    stage('BUILD') {
        sh 'mvn package'
    }
}