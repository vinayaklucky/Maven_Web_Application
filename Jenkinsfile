pipeline {
        agent any
        stages {
            stage('Checkout') {
                        steps {
                                git url: 'https://github.com/mddevopsaws/Maven_Web_Application.git'
                            }
         }
            stage('build') {
                        steps {
                                sh 'mvn clean package sonar:sonar'
                            }
         }
                }
}
