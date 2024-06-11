pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                dir('/var/lib/jenkins/workspace/pipeline_project-v1') {
                    git 'https://github.com/MinhPhamHP/test-jenkinsfile-1'
                    sh 'cp index.html index-testsh.html'
                    checkout changelog: false, poll: false, scm: scmGit(branches: [[name: '*/'+params.BRANCH ]], extensions: [], userRemoteConfigs: [[url: 'https://github.com/MinhPhamHP/test-jenkinsfile-1']])
                }
            }
        }
    }
}