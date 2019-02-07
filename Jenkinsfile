node{
  stage('SCM Checkout'){
    echo "code takes from SCM repository:"
    git 'https://github.com/Gopalkr78/my-app'
  }
  stage('Compile-Package'){
    sh 'mvn package'
  }
  
}
