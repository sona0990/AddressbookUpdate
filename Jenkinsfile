pipeline {
    agent any
    tools { 
        maven 'mymaven' 
        jdk 'myjdk' 
    }
    stages {
        stage('build') {
            steps {
                def mvnHome = tool 'Maven mymaven'
                sh "'${mvnHome}/bin/mvn' -Dmaven.test.skip=true clean package"
            }
        }
    }
}
