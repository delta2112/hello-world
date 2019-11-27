pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        def jenkinsfile = fileLoader.fromGit('test','git@github.com:delta2112/webproj.git','master',null,'')
        jenkinsfile.runJenkinsfile()
        sh '''#!/bin/sh

echo "DONE building"'''
      }
    }
  }
}

