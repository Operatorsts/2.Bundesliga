pipeline {
  agent any
  stages {
    stage('loesche alte Config') {
      steps {
        sh 'rm /var/lib/jenkins/2BL/configfile/fb98.cfg'
      }
    }

    stage('part1') {
      steps {
        sh '/var/lib/jenkins/2BL/configfile/part4.sh'
      }
    }

    stage('Spiel1 erstellen') {
      steps {
        sh '''/var/lib/jenkins/2BL/configfile/part3.sh 0 $SPIELNUMMER1 $ANLAGE1
'''
      }
    }

    stage('Spiel2 erstellen') {
      steps {
        sh '/var/lib/jenkins/2BL/configfile/part3.sh 1 $SPIELNUMMER2 $ANLAGE2'
      }
    }

    stage('Speil3 erstellen') {
      steps {
        sh '/var/lib/jenkins/2BL/configfile/part3.sh 2 $SPIELNUMMER3 $ANLAGE3'
      }
    }

    stage('Spiel4 erstellen') {
      steps {
        sh '/var/lib/jenkins/2BL/configfile/part3.sh 3 $SPIELNUMMER4 $ANLAGE4'
      }
    }

    stage('Spiel5 erstellen') {
      steps {
        sh '/var/lib/jenkins/2BL/configfile/part3.sh 4 $SPIELNUMMER5 $ANLAGE5'
      }
    }

    stage('Spiel6 erstellen') {
      steps {
        sh '/var/lib/jenkins/2BL/configfile/part3.sh 5 $SPIELNUMMER6 $ANLAGE6'
      }
    }

    stage('Spiel 7 erstellen') {
      steps {
        sh '''/var/lib/jenkins/2BL/configfile/part3.sh 6 $SPIELNUMMER7 $ANLAGE7
'''
      }
    }

    stage('Spiel8 erstellen') {
      steps {
        sh '''/var/lib/jenkins/2BL/configfile/part3.sh 7 $SPIELNUMMER8 $ANLAGE8
'''
      }
    }

    stage('Spiel9 erstellen') {
      steps {
        sh '''/var/lib/jenkins/2BL/configfile/part3.sh 8 $SPIELNUMMER9 $ANLAGE9
'''
      }
    }

    stage('part2') {
      steps {
        sh '/var/lib/jenkins/2BL/configfile/part2.sh $VAR_RUNDE $VAR_JAHR $VAR_ART'
      }
    }

    stage('step3') {
      steps {
        sh '/var/lib/jenkins/2BL/configfile/part1.sh'
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
    VAR_ART = '52'
    VAR_RUNDE = '18'
    VAR_JAHR = '01.01.2021'
  }
}