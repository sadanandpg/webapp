pipeline{
  
  agent any
  
  stages{
    
    stage("build")
    {
      steps
      {
      echo "building web application 1"
      }
    }
    stage("test")
    {
      steps
      {
      echo "testing web application 1"
      }
    }
    stage("deploy")
    {
      steps
      {
      echo "deploying web application 1"
      }
    }
    
  }
  post{
    always
    {
      echo "after stages web application 1"
    }
    
  }
  
}
