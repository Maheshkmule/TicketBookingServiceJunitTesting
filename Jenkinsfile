pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
             
                bat "git clone https://github.com/Maheshkmule/TicketBookingServiceJunitTesting.git"
                bat "mvn clean"
            }
        }
        stage('install') {
            steps {
                bat "mvn install"
                echo "Installing the maven---------"
            }
        }
        stage('test') {
            steps {
                bat "mvn test"
                echo "testing the maven---------"
            }
        }
        stage('package') {
            steps {
                bat "mvn package"
                echo "packaging the maven---------"
            }
        }
    }
}
