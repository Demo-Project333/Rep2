properties([
    [$class: 'GithubProjectProperty',
    displayName: '',
    projectUrlStr: 'https://github.com/Demo-Project333/Rep2.git/'],
    pipelineTriggers([upstream(upstreamProjects: "https://github.com/Demo-Project333/Rep1.git", threshold: hudson.model.Result.SUCCESS),githubPush()])])

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
