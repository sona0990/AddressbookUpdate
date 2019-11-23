pipeline {
    agent any
    tools { 
        maven 'mymaven' 
        jdk 'myjdk' 
    }
    stages {
        stage('build') {
            steps {
                script{
                env.Java_HOME= tool name: 'myjdk', type: 'jdk'
                def mvnhome = tool name: 'mymaven', type: 'maven'
                sh "'${mvnhome}/bin/mvn' package"
                }
            }
        }
    }
}
