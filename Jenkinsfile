pipeline {
  agent any
  stages {
    stage('Git pull') {
      steps {
        echo 'hi '
      }
    }

    stage('sonar') {
      steps {
        echo 'checking sonar'
      }
    }

    stage('building project') {
      parallel {
        stage('building project') {
          steps {
            echo 'building'
          }
        }

        stage('unit test') {
          steps {
            echo 'testing'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploying'
      }
    }

  }
}