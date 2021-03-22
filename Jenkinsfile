pipeline {
    agent any
    environment {
        PATH = "/usr/share/maven/bin:$PATH"
    }
    stages {
        stage("clone code"){
            steps{
               git credentialsId: 'neel8989', url: 'https://github.com/neel8989/cicd-maven-helloworld'
            }
        }
        stage("build code"){
            steps{
              sh "mvn clean install"
            }
        }
        
    }
}
