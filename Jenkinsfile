pipeline {
	agent any
	stages {
	stage('Checkout code') {
		steps {
			git branch: 'main', url: 'https://github.com/pathakbhaskar/batch-512.git'
	}
	}
		stage('Install Apache') {
		steps {
			sh 'sudo apt install apache2 -y'
	}
}
		stage('Deploy code') {
		steps {
			sh 'sudo cp -R * /var/www/html/'
	}
}
}
}
