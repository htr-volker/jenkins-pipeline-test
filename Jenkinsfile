pipeline {
    agent any
    stages {
        stage('What branch is it?') {
            steps {
                script {
                    if (env.BRANCH_NAME.contains('feature')) {
                        sh "echo This is a feature branch"
                    } else {
                        sh "echo This is not a feature branch"
                    }
                }
            }
        }
    }
}