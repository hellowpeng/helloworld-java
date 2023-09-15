pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo Build'
      }
    }

    stage('unit') {
      parallel {
        stage('Unit') {
          steps {
            sh 'echo UnitTest'
          }
        }

        stage('Performance') {
          steps {
            sh 'echo Performance'
          }
        }

      }
    }

    stage('Analyze') {
      steps {
        sh 'echo Analyze'
      }
    }

    stage('Deploy') {
      steps {
        sh 'echo Deploy'
      }
    }

  }
}