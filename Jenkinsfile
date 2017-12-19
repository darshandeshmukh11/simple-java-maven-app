pipeline {
    agent any
    env.JAVA_HOME = "${tool 'JDK 8'}"
    env.MAVEN_HOME = "${tool 'Maven 3.3'}"
    env.PATH = "${env.JAVA_HOME}/bin:${env.MAVEN_HOME}/bin:${env.PATH}"
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}
