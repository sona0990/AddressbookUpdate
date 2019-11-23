pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh "'${mvnHome}/bin/mvn' -Dmaven.test.skip=true clean package"
            }
        }
    }
}
