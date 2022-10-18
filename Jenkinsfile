pipeline {
    agent any
    
    stages {
        stage("Git pull") {
            steps {
                git url: "https://github.com/jenkins-getting-started/jgsu-spc-jenkinsfile.git", branch: "main"
            }
        }

        stage("Build") {
            steps {
                bat ".\\mvnw clean package"
            }

            post {
                
            }
        }
    }
}