pipeline {
    agent any

    stages {
        stage('Demo_2_build') {
            steps {
                build 'Demo_2'
            }
        }
        stage('Demo_4_build') {
            steps {
                build 'Demo_4'
            }
        }
        stage('demo_1_build') {
            steps {
                build 'demo_1'
            }
        }
        stage('cat README') {
            when{
                branch "Pratik-*"
            }
            steps {
                bat'''
                type README.md
                '''
            }
        }
    }
}
