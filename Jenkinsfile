properties([[$class: 'GithubProjectProperty', 
           displayName: '',
           projectUrlStr: 'https://github.com/Demo-Project333/'], 
           pipelineTriggers([upstream('Rep1'),githubPush()])])

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
                echo "This is a Test Stage" 
            }
        }
        stage('Deploy') {
            steps {
                echo "This is a Deploy Stage"
            }
        }
    }
}
