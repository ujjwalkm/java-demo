pipeline {
 
agent { node { label 'master' } }
tools {
        maven 'MAven3.3.9'
        jdk 'jdk1.8'
    }
stages {
        stage('Code validate') {
            steps {
                sh 'mvn validate'
            }
        }
        stage('Code Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('Code Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Code Package') {
            steps {
                sh 'mvn package'
            }
        }
 
       
    }
}
