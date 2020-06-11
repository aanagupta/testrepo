node {
stage('Build') {
  script {
	echo Creating test file > /tmp/test.$$
  }
 }
stage('Test') {
 script {
	if [ -e /tmp/test.$$ ]
        then
          echo found
        else
          echo Not Found
 }
}
}
