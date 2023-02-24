pipeline {
    agent any

    stages {
        stage('1-Build') {
           steps {
               echo  "Start of Stage Build"
               echo  "Building.............."
               echo  "End of Stage Build"
           }
        }
        stage('1-Test') {
           steps {
               echo  "Start of Stage Test"
               echo  "Testing.............."
               sh "ls"
               sh "pwd"
               sh "whoami"
               echo  "End of Stage Test"
           }
        }
        stage('1-Deploy') {
           steps {
               echo  "Start of Stage Deploy"
               echo  "Deploying.............."
               echo  "End of Stage Deploy"
           }
        }
    }
}
