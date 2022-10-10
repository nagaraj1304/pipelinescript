pipeline 
{
    agent any

    stages
     {
        stage('build')
         {
            steps 
            {
                echo 'build World'
            }
        }
    stage('test')
         {
            steps 
            {
                echo 'test World'
            }
        }
    stage('deploy')
         {
            steps 
            {
                echo 'deploy World'
            }
        }
     }      
      post 
      {
        failure
         {
        emailext body: 'code running summary', subject: 'pipelinescript', to: 'nagaraj04nani@gmail.com'
        }
      } 
  }
