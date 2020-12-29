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
        sh 'sonar ghhjgjh m,bkjbjb jkbjk'
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