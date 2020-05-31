pipeline { 
    agent any
    environment {
        AWS_DEFAULT_REGION = 'eu-west-1'

    }

    options {
		buildDiscarder(logRotator(numToKeepStr: '50', artifactNumToKeepStr: '50'))
		disableConcurrentBuilds()
		timestamps()
		timeout 240 // minutes
		ansiColor('xterm')
		skipDefaultCheckout()
    }

    stages {
        stage ('Proceed AMI Build') {
            steps{
                 input 'Build AMI?'
            }
        }
    }
}
