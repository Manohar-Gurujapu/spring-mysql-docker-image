pipeline {
    agent any
    tools{
        maven 'maven_3_9_1'
}
    stages {
        stage('Build') {
            steps {
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Manohar-Gurujapu/spring-mysql-docker-image']])
                sh 'mvn clean install'
            }
        }
      }
   }

