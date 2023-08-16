pipeline {
        agent any
            tools {
                    maven 'Maven'
            }
            stages {
                stage('git clone') {
                        steps {
                           git 'https://github.com/preethi-077/jenk.git'
                        }
                }
                stage('compile') {
                        steps {
                            sh 'mvn compile'
                        }
                }
                stage('test') {
                        steps {
                            sh 'mvn test'
                        }
                }
            }
}
