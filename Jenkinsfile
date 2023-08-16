pipeline   //the task which we are achieving
{
        agent any
            tools {
                    maven 'maven'
          }
        stages {
                stage('git clone') {
                        steps {
                           git 'https://github.com/ajit40/maven-integration-sak.git'
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
