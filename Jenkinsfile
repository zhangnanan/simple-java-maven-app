pipeline {
    agent {
        docker {
            image 'maven:3-alpine' 
            args '-u root' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}