pipeline {
    agent any

    tools {
        maven "M2_HOME"
    }

    stages {
        stage('Build') {
            steps {
                timeout(time: 5, unit: 'MINUTES') {
                    bat 'mvn -version'
                }
            }
        }
    }

    post {
        always {
            echo "======always======"
        }
    }
}
