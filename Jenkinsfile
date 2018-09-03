pipeline {

agent any
  
environment {
    DOCKER_COMMON_CREDS = credentials('jenkins-bitbucket-common-creds')
}

  stages {
    
    
    // Stage 1
    stage("Init"){
       steps
      {
        sh 'echo "Initialize"'
        sh 'docker login -u $DOCKER_COMMON_CREDS_USR -p $DOCKER_COMMON_CREDS_PSW'
      }
    }
    
    // Stage2
    
    stage("Build"){
       steps
      {
        sh 'docker build .'
      }
    }
    
    //
    
    
    

  }


}
