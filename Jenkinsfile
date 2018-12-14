pipeline {
   agent any
   stages {
   stage ('Checkout') {
steps {
checkout scm
   sh "yum install -y maven"
   sh "mvn clean install"
}
}  
   stage ('Build') {
     steps {
          echo "HelloWorld"
          }
  }
}
}
