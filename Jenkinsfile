pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package -Dmaven.test.skip=true'
            }
        }
        stage('Run') {
            steps {
                sh 'java -jar target/my-app-new-1.0-SNAPSHOT.jar'
            }
        }
    }
}
