pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'i want to build'
        git(url: 'https://github.com/balkrushna4645/Oceanblue.git', branch: 'main')
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'i want to test'
          }
        }

        stage('Deploy') {
          steps {
            echo 'i want to Deploy'
          }
        }

      }
    }

  }
}