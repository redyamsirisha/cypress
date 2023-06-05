pipeline{
    agent {
        dockerfile {
            filename 'Dockerfile'
            args '-u root:root'
        }
    }
    stages { 
      stage("build npm dependencies"){
        steps{
          checkout scm
          sh '''npm ci'''
        }
      }  
    }
}
