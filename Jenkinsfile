pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh '''echo "Hello World"
echo "Multi line shell steps works too"
ls -lah
pwd'''
          }
        }
        stage('Development') {
          steps {
            sh 'tidy -q -e index.html'
          }
        }
      }
    }
  }
}