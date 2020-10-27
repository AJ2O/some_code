pipeline {
  agent any
  stages {
    stage('echo') {
      steps {
        echo 'hello from the trigger'
        echo 'Hello Again'
	echo 'Hello from the trigger again'
      }
    }

    stage('echo part 2') {
      steps {
        sh 'hostname'
      }
    }

  }
  triggers {
    cron('H/15 * * * *')
  }
}
