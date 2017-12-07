properties([[$class: 'GithubProjectProperty', 
           displayName: '',
           projectUrlStr: 'https://github.com/Demo-Project333/'], 
       pipelineTriggers([upstream(threshold: 'SUCCESS',upstreamProjects: 'https://github.com/Demo-Project333/Rep1.git')])])

pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                echo " This is Build Stagee"
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
