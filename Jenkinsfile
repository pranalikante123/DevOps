pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                echo 'hello world'
            }
        }
        stage('deploy') {
            steps {
                bat 'systeminfo '
            }
        }
        stage('compile') {
            steps {
                echo 'systeminfo '
            }
        }
        stage('build') {
            steps {
                echo 'systeminfo '
                env.GIT_COMMIT = sh(script: "git rev-parse HEAD ", returnStdout: true).trim() 
				println "${env.GIT_COMMIT}"
            }
        }
    }
}

