pipeline {
    agent {label 'swarm'}
    stages {
        stage('GradleBuild') {
            steps {
                sh './gradlew build --no-daemon'
            }
        }
        stage('GradleTest') {
            steps {
                sh './gradlew clean test --no-daemon'
            }
        }
    }
}
