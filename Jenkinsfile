pipeline {
    agent any
    stages {
        stage('Which Branch Is It Anyway?') {
            steps {
                script {
                    if (env.GIT_BRANCH.contains('main')) {
                        sh "echo This is the main branch! Full name: $GIT_BRANCH"
                    }
                    else if (env.GIT_BRANCH.contains('dev')) {
                        sh "echo This is the dev branch! Full name: $GIT_BRANCH"
                    }
                    else if (env.GIT_BRANCH.contains('feature')) {
                        sh "echo This is a feature branch! Full name: $GIT_BRANCH"
                    } 
                    else {
                        sh "echo This branch is named: $GIT_BRANCH"
                    }
                }
            }
        }
    }
}
