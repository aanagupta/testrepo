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
		sh '/bin/uptime'
		}
         }
        stage('Deploy') {
	   when {
	  expression {
		 currentBuild.result == null || currentBuild.result == 'SUCCESS'
                }
              }
           steps {
       		sh 'echo "Deployment Done"'
     	        }
    	 }
  	}
}
