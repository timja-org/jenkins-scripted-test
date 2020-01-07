node {
  stage('Checkout') {
    checkout scm
  }
  
  stage('Build') {
    sh "env | egrep 'GIT|CHANGE'"
  }
  
  stage('Notify') {
   slackSend notifyCommitters: true, message: "Build done"
  }
  
}
