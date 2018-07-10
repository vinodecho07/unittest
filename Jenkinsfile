pipeline {
  agent any

  stages {
    stage {
      steps ('Test') {
	sh 'ant test'
      }
    }
    stage {
      steps ('Build') {
        sh 'ant build'
      }
    }
    stage {
      steps ('Deploy') {
        sh 'cp dist/*.war /tmp'
      }
    }
  }
}

