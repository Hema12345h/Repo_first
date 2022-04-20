pipeline 
{
    agent any
    stages 
  {
        stage('Build') 
      {
            steps
           {
                echo 'Build App : %date% : %time%'
            }
        }
    
       stage('Test') 
      {
            steps
           {
                echo 'Test App : %date% : %time%'
            }
        }
       stage('Deploy') 
      {
            steps
           {
                echo 'Deploy App: %date% : %time%'
            }
        }
    
      }
  post
  {
    always
    {
      emailext body: 'Job', subject: 'Jenkins job', to: 'hemas5aws@gmail.com'
    }
  }
  
  
 
}

