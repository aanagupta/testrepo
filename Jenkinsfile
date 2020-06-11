pipeline {
agent any 
	stages {
	stage('Build') { 
	   steps { 
		sh '/usr/bin/ls' 
	        }
	 }
        stage('Test'){
	   steps {
		sh 'make check'
		}
         }
        stage('Deploy') {
           steps {
       		sh 'make publish'
     		}
    	 }
  	}
}
