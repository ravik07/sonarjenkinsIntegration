pipeline {
        agent none
        stages {
         
          stage("build & sonarqube") {
            agent any
            steps {
              withSonarQubeEnv('MySonar') {
                bat 'mvn clean package sonar:sonar'
              }
            }
          }
        }
      }
