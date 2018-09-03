pipeline {

agent any
  
environment {
    DOCKER_COMMON_CREDS = credentials('a05e481d-4987-4a51-8569-41fc1a47e11e')
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
