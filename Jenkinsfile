pipeline {
  agent any
  
  stages {
    stage('build') {
      steps {
        sh 'ajavc -d . src/*.java'
        sh 'echo Main-CLASS: Rectanulator > MANIFEST.MF'
        sh 'jar -cvmf MANIFEST.MF rectangle.jar *.class'
        }
    }
  }
}
