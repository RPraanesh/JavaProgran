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
      sh "yum install -y maven"
      sh "maven clean install"
    archiveArtifacts artifacts: 'dist/sampleapp.zip'
      }
    }
  }
}
}
