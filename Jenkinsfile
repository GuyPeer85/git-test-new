pipeline {
  agent any
  stages {
    stage('hello') {
      steps {
        echo 'hello world'
        sh '$PWD'
      }
    }

    stage('sleep') {
      steps {
        sleep 4
      }
    }

    stage('step1') {
      steps {
        writeFile(file: 'test1.txt', text: 'echo "step1"')
      }
    }

  }
  environment {
    guy = '1'
  }
}