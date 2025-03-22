pipeline {
    agent saigonsky
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/user/repo.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                // Chạy lệnh build, ví dụ với Maven
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Ví dụ deploy lên server
                sh 'scp target/*.jar user@server:/deploy/'
            }
        }
    }
}
