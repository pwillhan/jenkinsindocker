def gv
pipeline {
  agent any
  stages {
    stage("init") {
      steps {
        script {
          gv = load "script.groovy"
        }
      }
    }
    stage("build") {
      steps {
        script {
          gv.buildApp()
        }
      }
    }
    stage("test") {
      steps {
        echo 'testing'
      }
    }
    stage("deploy") {
      steps {
        echo 'deploying'
      }
    }
  }
}
