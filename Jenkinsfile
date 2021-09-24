pipeline {
  agent any 
    stages {
      stage ("SCM") {
        steps {
          git credentialsId: 'pavan_github', url: 'https://github.com/pavanpasila/Test-Repo.git'
        
        }
      }
    }
}

