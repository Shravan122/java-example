pipeline{
agent none
	stages {
	  stage('GIT checckout') {
	  agent {label 'slave-1'}
		steps {
		  echo 'This is Checkout stage'
		}
	  }

	  stage('Build') {
	  agent {label 'slave-1'}
		steps {
			echo 'This is Build stage'
		}
	  }

	  stage('Push') {
	  agent {label 'slave-2'}
		steps {
		  echo 'This is push stage'
		}
	  }

	  stage('Deploy') {
	  agent {label 'slave-2'}
		steps {
		  echo 'This is Deploy stage'
		}
	  }

	}
}	
