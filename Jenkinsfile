pipeline {
    agent any
stages {
    stage('Tests') {
        steps {
            sh 'echo Running tests'
    }
}
stages {
    stage('Approve') {
        input message: 'Tests passed. Deploy to production?'
    }
}
stages {
    stage('Deploy') {
        steps {
            sh 'echo Deploying to production'
        }
    }
}
