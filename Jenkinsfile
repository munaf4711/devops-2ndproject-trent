pipeline {
    agent {
        node {
            label'maven'
        }
    }

    stages {
        stage('clone the code from github') {
            steps {
                git branch: 'main', url: 'https://github.com/munaf4711/Devops-project-2-trend.git'
            }
        }
    }
}

