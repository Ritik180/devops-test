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
 }
}
