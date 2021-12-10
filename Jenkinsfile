pipeline {
  agent any
  stages {
    stage('loesche alte Config') {
      steps {
        sh 'rm /var/lib/jenkins/2BL/configfile/fb98.cfg'
      }
    }

    stage('erstelle config part1') {
      steps {
        sh '/var/lib/jenkins/2BL/configfile/part1.sh'
      }
    }

  }
}