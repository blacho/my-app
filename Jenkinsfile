node{
  stage('SCM Checkout'){
    git 'https://github.com/blacho/my-app'
  }
  stage('Complie-Package'){
    def mvnHome = tool name: 'maven-3', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
  stage('Email notification'){
    mail bcc: '', body: '''Hi
Welcome to Jenkis email alerts!
Thanks
Irek''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'irek_b@wp.pl'
}
