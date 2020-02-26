pipeline {
    agent any
    tools {
        jdk 'jdk1.8.0_121'
        maven 'maven-3.0.4'
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'mvn --settings /jetn/app/tools/apache-maven-3.0.4/conf/serviceaccount_jenkinsgithub-settings.xml -U clean deploy'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
