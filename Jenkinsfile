node('OPENMRS') {
    stage('VCS') {
        git url: 'https://github.com/Shoaib-23/openmrs-core.git',
            branch: 'scripted'    
    }
    stage('BUILD') {
        def mvnTool = tool 'MAVEN-3.9.0'
        sh "${mvnTool}/bin/mvn clean install"
    }
}
