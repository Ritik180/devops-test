pipeline {
  agent any{
    stages{
      stage('build stage'){
        steps{
         withMaven(maven : 'maven_3_5_0') {
                    sh 'mvn clean install'
         }
        }
      }
    }
  }
}
