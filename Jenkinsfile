pipeline{
 agent any
 
 stages {
 	stage ('Build'){
 		steps {
 			withMaven(maven:'maven'){
 				bat 'mvn clean install'
 			}
 		}
 	}
 }
}
