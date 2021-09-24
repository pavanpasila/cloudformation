pipeline {
  agent any 
    stages {
      stage ("SCM") {
        steps {
          git credentialsId: 'pavan_github', url: 'https://github.com/pavanpasila/Test-Repo.git'
        }
      }
      stage ("Launch Cloud Formation Stack") {
        steps {
          sh "aws configure list"
          sh  "aws cloudformation create-stack --stack-name myteststack --template-body file://cfn/s3.template --capabilities CAPABILITY_IAM"    
        
        }
      }
    }
}

