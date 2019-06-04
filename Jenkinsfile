pipeline {

    agent any

    tools {
        maven 'LocalMaven'
    }


	triggers {
        issueCommentTrigger('.*test this please.*')
    }

    stages{

        stage('Build'){

            steps {

                bat 'mvn clean package'

            }

        }


    }

}