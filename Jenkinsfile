properties([[$class: 'GithubProjectProperty', 
           displayName: '',
           projectUrlStr: 'https://github.com/Demo-Project333/Rep2.git/'], 
           pipelineTriggers([githubPush()])])

pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                echo " This is Build Stage"
            }
        }
        stage('Test'){
            steps {
                echo "This is a Test Stagee" 
            }
        }
        stage('Deploy') {
            steps {
                echo "This is a Deploy Stage"
            }
        }
    }
}
