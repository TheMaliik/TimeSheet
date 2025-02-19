pipeline {
    agent any

    tools {
        jdk 'JAVA_HOME'
        maven 'MAVEN_HOME'  // Change here from 'M2_HOME' to 'MAVEN_HOME'
    }

    stages {
        stage('GIT') {
            steps {
                git branch: 'master', 
                    url: 'https://github.com/TheMaliik/TimeSheet.git'
            }
        }

        stage('Compile Stage') {
            steps {
                sh 'mvn clean compile'
            }
        }
    }
}
