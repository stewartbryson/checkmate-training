#!/usr/bin/env groovy

def options = '-Si'
def properties = "-PbuildId=${env.BUILD_TAG}"
def checkmate = "./gradlew ${options} ${properties}"

pipeline {
    agent {
        label 'master'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Publish') {
            steps {
                echo 'Building..'
            }
        }
        stage('Deploy') {
            when {
                branch 'master'
             }
            steps {
                echo 'Deploying..'
            }
        }
    }
}