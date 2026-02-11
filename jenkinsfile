pipeline {
    agent any

    tools {
        jdk 'JAVA_HOME'
        maven 'M2_HOME'
    }

    stages {
        stage('Compile and Test') {
            steps {
                // On utilise 'sh' pour Linux. Si Jenkins est sur Windows, utilisez 'bat'
                sh 'mvn clean install -DskipTests'
            }
        }
    }
}