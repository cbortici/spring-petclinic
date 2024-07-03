pipeline {
    agent any
    tools {
        maven 'mvn' 
    }
    stages {
        stage('Example') {
            steps {
                sh '''
                cd spring-petclinic
                mvn -B -DskipTests clean package
              
                      '''
            }
        }
    }
}
