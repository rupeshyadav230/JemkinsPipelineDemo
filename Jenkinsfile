pipeline {
    agent any

    stages {
        stage('Git Clone') {
            steps {
                git credentialsId: 'GIT_HUB_CREDENTIALS', url: 'https://github.com/rupesh-zcr/springboot-with-docker.git'
            }
        }
     stages {
       stage('Gradle Build') {
           steps {
               sh './gradlew build'
           }
       }
        
    }
}
}
