pipeline {
    agent {
        node {
            label 'maven'
        }
    }

environment {
    PATH = "/opt/apache-maven-3.9.11/bin:$PATH"
}
    stages {
        stage('Check dump file') {
    steps {
        sh 'cat target/surefire-reports/*.dumpstream || true'
    }
}
       stage('build') {
         steps {
            sh 'mvn clean deploy'
         }
    }

   }
}
