pipeline {
    agent { label 'test' }
    tools {
        maven 'mvn'
        jdk 'jdk17'
    }
    stages {
        stage('Example') {
            steps {
                sh '''
                docker build -t helloworld/pet-clinic .
                mvn -B -DskipTests clean package
                java -jar /home/jenkins/workspace/example/spring/target/spring-petclinic-3.3.0-SNAPSHOT.jar
                      '''
            }
        }
    }
}
