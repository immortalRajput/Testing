pipeline
{
    agent any
    stages{
    stage ("Download code")
    {
        steps
        {
            git url: 'https://github.com/immortalRajput/webapp.git' , branch: 'master'
            
        }
        
    }
    stage ("Scan code")
    {
        steps
        {
          sh ' trivy fs . '
            
        }
        
    }
    
    }
}
