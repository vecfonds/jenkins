pipeline {
    agent {
        label 'saigonsky'
    }
    stages {
        stage('Info') {
            steps {
                echo 'Testing...'
                sh( """ whoami;pwd;ls -la """, label: "test")
            }
        }
    }
}
