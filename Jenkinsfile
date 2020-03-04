pipeline{
 agent any
 
 stages {
 	stage ('Build'){
 		steps {
 			withMaven(maven:'maven'){
 				bat 'mvn -f mule-jenkins-pipeline/pom.xml clean install'
 			}
 		}
 	}
 }
}
