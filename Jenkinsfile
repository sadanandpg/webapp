pipeline{
  
  agent any
  environment{
      NEW_VERSION='1.3.0'
  }
  
  stages{
    
    stage("build")
    {
      steps
      {
      echo "building web application 2"
      echo "version is ${NEW_VERSION}"
      }
    }
    stage("test")
    {
      steps
      {
      echo "testing web application 2"
      }
    }
    stage("deploy")
    {
      steps
      {
      echo "deploying web application 2"
      }
    }
    
  }
  post{
    always
    {
      echo "after stages web application 2"
    }
    
  }
  
}
