node{
  stage('SCM Checkout'){
    echo "code takes from SCM repository:"
    git 'https://github.com/Gopalkr78/my-app'
  }
  stage('Compile-Package'){
    def MVN_HOME = tool name: 'maven3', type: 'maven'
    sh "${MVN_HOME}/bin/mvn package"
  }
  stage('Email notification'){
    mail bcc: '', body: 'Hello this is first pipeline job!!!', cc: '', from: '', replyTo: '', subject: 'Code takes form source code repository', to: 'nasrealimage@gmail.com'
  }
  
}
