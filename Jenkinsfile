pipeline {
   agent any
   stages {
   stage ('Checkout') {
steps {
checkout scm
   sh "yum install -y maven"
   sh "maven clean install"
}
}
   stages {
   stage ('Build') {
     steps {
      
    archiveArtifacts artifacts: 'dist/sampleapp.zip'
      }
    }
  }
}
}
