node {
  stage('Checkout') {
    checkout scm
  }
  
  stage('Build') {
    sh "env | egrep 'GIT|CHANGE'"
  }
   
}
