pipeline {
    agent any
    tools { 
        maven 'mymaven' 
        jdk 'myjdk' 
    }
    stages {
        stage('build') {
            steps {
                
                sh "'${maven}/bin/mvn' -Dmaven.test.skip=true clean package"
            }
        }
    }
}
