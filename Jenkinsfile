// Using Jenkins to build a Java application with Maven

pipeline {
    agent {
        docker {
            image 'maven:3-alpine'
            //args '-v /root/.m2:/root/.m2'
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