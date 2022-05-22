pipeline{
  
  agent any
  environment{
      NEW_VERSION='1.3.0'
      SERVER_CREDENTIALS= credentials('server credentials')
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
      echo "version is ${SERVER_CREDENTIALS}"
      
      withCredentails(
          [
              usernamePassword(credentials:'server credentials', usernameVariable:USER,
              passwordVariable: PWD )
          ]
      )
      {
            echo "values ${USER}"
      }
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
