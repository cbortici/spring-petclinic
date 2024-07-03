pipeline {
    agent any
    tools {
        maven 'mvn'
        jdk 'jdk17'
    }
    stages {
        stage('Example') {
            steps {
                sh '''
                java version
                mvn -B -DskipTests clean package
              
                      '''
            }
        }
    }
}
