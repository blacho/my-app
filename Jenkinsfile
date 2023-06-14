node{
  stage('SCM Checkout'){
    git 'https://github.com/blacho/my-app'
  }
  stage('Complie-Package'){
    def mvnHome = tool name: 'maven-3', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
}
