/* groovylint-disable-next-line CompileStatic */
pipeline {
    agent any
  
    stages {
        /* stage('SCM Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/sagarkrp/fakeweb.git'
            //sh 'whoami'
            }
        } */

        stage('SonarScan') {
            steps {
                './gradlew sonar \
                    -Dsonar.projectKey=Gradle_Project \
                    -Dsonar.projectName='Gradle_Project' \
                    -Dsonar.host.url=http://localhost:9000 \
                    -Dsonar.token=sqp_e2497c7ad5f5ed82b3775e082efd2b770f7e6ba7'
            }
        }
    }
}