pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh './mvnw clean package -Dquarkus.kubernetes.deploy=true -Dquarkus.openshift.route.expose=true'
            }
        }
    }
}
