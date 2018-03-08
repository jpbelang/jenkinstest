pipeline {
    agent any
    stages {
        stage("Build") {
            steps {
                withMaven(
                        // Maven installation declared in the Jenkins "Global Tool Configuration"
                        mavenLocalRepo: '.repository') {

                    // Run the maven build
                    sh "mvn clean install"
                }
            }
        }
    }
}
