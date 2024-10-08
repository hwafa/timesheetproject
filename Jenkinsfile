pipeline {
    agent any
    tools {
        jdk 'JAVA_HOME'
        maven 'M2_HOME'
    }

    stages {
        stage('GIT') {
            steps {
                git branch: 'master', 
                    url: 'https://github.com/tamim-hmizi/timesheetproject.git',
                    credentialsId: '421f578a-8360-4777-a60b-926fec1d0647'
            }
        }

        stage('Compile Stage') {
            steps {
                bat 'mvn clean compile'
            }
        }
    }
}
