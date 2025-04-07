pipeline {
        agent none
        stages {
         
          stage("build & sonarqube") {
            agent any
            steps {
              withSonarQubeEnv('MySonar') {
                sh 'mvn clean package sonar:sonar'
              }
            }
          }
        }
      }