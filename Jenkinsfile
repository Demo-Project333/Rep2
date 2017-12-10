properties([
    [$class: 'GithubProjectProperty',
    displayName: '',
    projectUrlStr: 'https://github.com/Demo-Project333/Rep2.git'],
    pipelineTriggers([upstream('https://github.com/Demo-Project333/Rep1.git'),githubPush()])])

  ///  pipelineTriggers([upstream(threshold: hudson.model.Result.SUCCESS, upstreamProjects: 'https://github.com/Demo-Project333/Rep1.git/master')])])

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
