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
        sh '/var/lib/jenkins/2BL/configfile/part4.sh'
      }
    }

    stage('Spiel1 erstellen') {
      steps {
        sh '/var/lib/jenkins/2BL/configfile/part3.sh 0 SPIELNUMMER1 ANLAGE1'
      }
    }

  }
  environment {
    SPIELNUMMER1 = '180201'
    ANLAGE1 = '3'
    SPIELNUMMER2 = '180202'
    ANLAGE2 = '5'
    SPIELNUMMER3 = '180206'
    ANLAGE3 = '4'
    SPIELNUMMER4 = '180214'
    ANLAGE4 = '3'
    SPIELNUMMER5 = '180233'
    ANLAGE5 = '8'
    SPIELNUMMER6 = '#'
    ANLAGE6 = '#'
    SPIELNUMMER7 = '#'
    ANLAGE7 = '#'
    SPIELNUMMER8 = '#'
    ANLAGE8 = '#'
    SPIELNUMMER9 = '#'
    ANLAGE9 = '#'
  }
}