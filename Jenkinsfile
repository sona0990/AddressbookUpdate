pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                def mvnHome = tool 'Maven mymaven'
                sh "'${mvnHome}/bin/mvn' -Dmaven.test.skip=true clean package"
            }
        }
    }
}
