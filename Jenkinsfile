node{
  stage('SCM Checkout'){
    git 'https://github.com/blacho/my-app'
  }
  stage('Complie-Package'){
    sh 'mvn package'
  }
}
