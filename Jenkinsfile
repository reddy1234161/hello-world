pipeline {
    agent { 
    stages {
         stage('scm') {
            steps {
               git credentialsId: 'github', url: 'https://github.com/reddy1234161/hello-world.git'
            }
        }
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
