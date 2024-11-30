pipeline {
    agent {
        label 'docker-slave'
    }
    environment {
        DATABASE = 'DOCKER'
    }
    stages {
        stage ('this is maven build stage # 1') {
            when {
                expression {
                     branch_name ==~ /(feature|hotfix)/
                }
            }
            steps {
                echo "this stage is executed from feature branch"

            }
        }
    }
}
