node{
  stage('SCM Checkout'){
    echo "code takes from SCM repository:"
    git 'https://github.com/Gopalkr78/my-app'
  }
  stage('Compile-Package'){
    def MVN_HOME = tool name: 'maven3', type: 'maven'
    sh "${MVN_HOME}/bin/mvn package"
  }
  
}
