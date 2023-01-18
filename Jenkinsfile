pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Build') {
            steps {
                echo 'Building'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing'
                snykSecurity snykInstallation: 'Synk_Security', snykTokenId: 'snyk-jenkins', targetFile: 'infoProject'
            }
        }
        stage('Release') {
            steps {
                echo 'Releasing'
            }
        }
    }
}
