pipeline {
    agent any

    stages {
        stage('Load Updated playbook') {
            steps {
                git 'https://github.com/dnmwangi/ansible_lab.git'
                slackSend channel: '#jenkins-notifications', failOnError: true, message: 'Stage1 : Playbook load successfull', teamDomain: 'ust-fzr2841.slack.com'
                echo 'Playbook Load Successfull'
            }
        }
        stage('Unit Testing') {
            steps {
                echo 'This is unit testing '
            }
        }
        stage('Function Testing') {
            steps {
                echo 'This is function testing'
            }
        }
        stage('Integration Testing') {
            steps {
                echo 'This is Integration testing'
            }
        }
        stage('Deploy to production') {
            steps {
                echo 'This is production Deployment'
            }
        }
    }
}
