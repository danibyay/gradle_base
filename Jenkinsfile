pipeline {
    agent {label 'swarm'}
        stages {
            stage('GradleTest') {
                steps {
                    sh './gradlew build'
                    sh './gradlew clean test --no-daemon'  
                }
            }
        }
    }
