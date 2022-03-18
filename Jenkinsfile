pipeline {
  agent any

  tools {
	nodejs 'nodejs'
	}

  stages {
    stage('compile-app') {
      steps {
        echo 'this is the compile job'
        sh 'npm install'
      }
    }
    stage('test-app') {
      steps {
        echo 'this is the test job'
        sh 'npm test'
      }
    }
    stage('package-app') {
      steps {
        echo 'this is the package job'
        sh 'npm run package'
      }
    }
  }
}
  post {
    always {
      echo 'Standard Templated Pipeline'
    }

  }
}
