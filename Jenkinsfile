pipeline {
    agent any
    stages {
        stage('What branch is it?') {
            steps {
                script {
                    when (env.BRANCH_NAME.contains('feature')) {
                        echo "This is a feature branch"
                    } else {
                        echo "This is not a feature branch"
                    }
                }
            }
        }
    }
}