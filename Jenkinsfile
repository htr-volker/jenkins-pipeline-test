pipeline {
    agent any
    stages {
        stage('What branch is it?') {
            steps {
                script {
                    if (env.GIT_BRANCH.contains('feature')) {
                        sh "echo This is a feature branch! It\'s $GIT_BRANCH"
                    } else {
                        sh "echo This is not a feature branch! It\'s $GIT_BRANCH"
                    }
                }
            }
        }
    }
}