node {
    docker.image('node:16-buster-slim').inside('-p 3000:3000') {
		//build stage
        stage('Build') {
			//eksekusi build
            sh 'npm install'
        }
		
		//test stage
        stage('Test') {
			//eksekusi test
            sh './jenkins/scripts/test.sh'
        }
    }
}
