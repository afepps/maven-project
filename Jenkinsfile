pipeline {

    agent any

    tools {
        maven 'LocalMaven'
    }


	triggers {
        githubPullRequest {
            cron('H/5 * * * *')
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