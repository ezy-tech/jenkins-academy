pipeline {
    agent { 
        node {
            label 'docker-alpine-agent'
            }
      }
    stages {
        stage('clone') {
            steps {
                echo 'cloning repo (scm)'
            }
            
        }
        stage('build') {
            steps {
                echo 'building code'
                
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
        stage('test') {
            steps {
                echo 'testing code'
            }
        }
        stage('packaging') {
            steps {
                echo 'packaging code'
            }
        }
        stage('deploying') {
            steps {
                echo 'deploying code'
            }
        }
    }
}
