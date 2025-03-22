pipeline {
    agent {
        label 'saigonsky'
    }
    stages {
        stage('Info') {
            steps {
                echo 'Testing...'
                sh(script: """ whoami;pwd;ls -la """, label: "test xxxxxx")
            }
        }
    }
}
