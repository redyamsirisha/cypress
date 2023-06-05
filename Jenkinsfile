pipeline{
    agent {
        dockerfile {
            label 'linux'
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
