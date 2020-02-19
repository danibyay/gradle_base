pipeline {
    agent {label 'swarm'}
    stages {
        stage('GradleBuild') {
            steps {
                sh './gradlew build'
            }
        }
    }
}
