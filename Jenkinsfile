pipeline {
    agent any
    stages {
        stage('Step 1 Packaging') {
            steps {
              sh "mvn clean pack"
            }
        }
		stage('Step 2 archive artifacts') {
            steps {
             archiveArtifacts artifacts: '**/*.war', fingerprint: true
            }
        }
}
}
