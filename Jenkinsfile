pipeline {

    agent any

    tools {
        maven 'LocalMaven'
    }


	triggers {
        githubPullRequests(),
		githubPush()
    }

    stages{

        stage('Build'){

            steps {

                bat 'mvn clean package'

            }

        }


    }

}