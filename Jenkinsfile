pipeline {
    agent { docker { image 'maven:3.3.3' } }
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
