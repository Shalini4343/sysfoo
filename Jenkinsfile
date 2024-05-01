pipeline {
    agent any
    stages {
        stage('Step   #01 Packaging') {
            steps {
              sh "mvn clean package"
            }
        }
		stage('Step 2 archive artifacts') {
            steps {
             archiveArtifacts artifacts: '**/*.war', fingerprint: true
            }
        }
}
}
