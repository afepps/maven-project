pipeline {

    agent any

    tools {
        maven 'LocalMaven'
    }


	triggers {
        githubPull(),
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