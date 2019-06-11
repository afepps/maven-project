pipeline {

    agent any

    tools {
        maven 'LocalMaven'
    }


	triggers {
        githubPullRequest {
           
            useGitHubHooks()
            
        }
    }

    stages{

        stage('Build'){

            steps {

                bat 'mvn clean package'

            }

        }


    }

}