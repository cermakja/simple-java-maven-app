pipeline {
    agent {
        docker {
            image 'maven:3-alpine' 
            args '-v "C:\Users\cermakja\OneDrive - MATTEL INC\Projects\Docker\jenkins\.m2":/root/.m2' 
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
