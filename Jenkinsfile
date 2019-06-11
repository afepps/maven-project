pipeline {

    agent any

    tools {
        maven 'LocalMaven'
    }


	triggers {
        githubPullRequests (
            triggerMode('Cron with Persisted Data')
            crontabline('H/5 * * * *')
            triggerEvents('Pull Request Opened')
            
        )
    }

    stages{

        stage('Build'){

            steps {

                bat 'mvn clean package'

            }

        }


    }

}