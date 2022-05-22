pipeline{
  
  agent any
  
  stages{
    
    stage("build")
    {
      steps
      {
      echo "building web application 2"
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
