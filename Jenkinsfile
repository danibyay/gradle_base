pipeline {
    agent {label 'swarm'}
        stages {
            stage('GradleBuild') {
                steps {
                    sh './gradlew build'
                }
            }
            stage('GradleTests') {
                steps {
                    sh './gradlew clean test --no-daemon'
                }
            }          
        }
}
