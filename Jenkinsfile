pipeline{
 agent any
 
 stages {
 	stage ('Build and Test Munit Test Cases'){
 		steps {
 			withMaven(maven:'maven'){
 				bat 'mvn clean install'
 			}
 		}
 	}
  stage ('Deploy to Cloudhub'){
   steps{
    withMaven(maven:'maven'){
     configFileProvider([configFile(fileId: 'config_deploy', variable: 'DEPLOY_SETTINGS')]) {
    bat 'mvn clean deploy'
}
    }
   }
  }
 }
}
