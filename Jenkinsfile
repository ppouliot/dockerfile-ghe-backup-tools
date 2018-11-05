def SUFFIX = ''

pipeline {
    agent any

    parameters {
        string (name: 'VERSION_PREFIX', defaultValue: '0.0.0', description: 'puppet-ipam version')
    }
    environment {
        BUILD_TAG = "${env.BUILD_TAG}".replaceAll('%2F','_')
        BRANCH = "${env.BRANCH_NAME}".replaceAll('/','_')
    }
    options {
        buildDiscarder(logRotator(numToKeepStr: '30'))
    }
    stages {
        stage ('Checkout and build dockerfile-ghe-helper.') {
            when {
              expression {
                currentBuild.result == null || currentBuild.result == 'SUCCESS' 
              }
            }
            steps {
                dir("${env.WORKSPACE}") {
                    sh './build.sh -d'
                }
            } 
        }

    } 
}
