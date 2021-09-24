pipeline {
  agent any 
    stages {
      stage ("SCM") {
        steps {
          git branch: 'main', credentialsId: 'pavan_github', url: 'https://github.com/pavanpasila/Test-Repo.git'
        
        }
      }
    }
}

