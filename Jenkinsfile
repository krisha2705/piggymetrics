pipeline{
agent any
	stages {
	
	   stage('SCM Checkout'){
	       steps {
	   bat "mvn clean"
	}
      }
	stage('Build Package'){
	     steps {
	     withMaven(maven : 'apache-maven-3.6.0')
	   {
	   bat 'set'
	   bat "mvn package"
	}
       }
       }
     }
}
