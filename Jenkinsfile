pipeline {
   agent any
   stages {
   stage('Checkout') {
steps {
dir('Java') {
git credentialsId: 'GITHUB', url: 'https://github.com/RPraanesh/Java'
}
}
}
   stages {
   stage ('Build') {
     steps {
    echo 'Running Build Automation '
    sh './gradlew build --no-daemon'
    archiveArtifacts artifacts: 'dist/sampleapp.zip'
      }
    }
  }
}
