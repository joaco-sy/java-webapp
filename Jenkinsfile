pipeline {
    tools {
        maven 'Maven'
    }
    stages {
        stage ('start') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                '''
            }
        }

        stage ('Build') {
            sh 'mvn clean package'
        }
    }
}