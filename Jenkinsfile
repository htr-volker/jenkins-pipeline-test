pipeline {
    agent any
    stages {
        stage('Which Branch Is It Anyway?') {
            steps {
                script {
                    if (env.GIT_BRANCH.contains('feature')) {
                        sh "echo This is a feature branch! It is $GIT_BRANCH"
                    } else {
                        sh "echo This is not a feature branch! It is $GIT_BRANCH"
                    }
                }
            }
        }
    }
}