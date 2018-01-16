pipeline {
    agent {
        docker {
            image 'maven:3.2-jdk-7' 
            args '-v /Users/tester/.m2:/root/.m2' 
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