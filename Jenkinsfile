pipeline {
    agent any
    stages {
        stage('Build') {
            steps{ echo 'Building '}
    }
    stage('Tests') {
        parallel {
            stage('Unit') { steps { sh 'echo Unit tests' } }
            stage('Integreation'){ steps { sh 'echo Integration tests' } }
        }
    }
}
}       
        
