pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                git 'https://github.com/MinhPhamHP/test-jenkinsfile-1'
                sh 'cp index.html index-testsh.html'
            }
        }
    }
}