pipeline {
    agent {label 'swarm'}
    stages {
        stage('GradleTest') {
            steps {
                sh 'chmod +x ./gradlew'
                sh './gradlew clean test --no-daemon'
            }
        }
        stage('GradleBuild') {
            steps {
                sh './gradlew build --no-daemon'
            }
        }
    }
}
