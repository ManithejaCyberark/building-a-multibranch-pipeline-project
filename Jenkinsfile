pipeline {
 agent any
 stages{
   stage("Git Checkout"){
    steps{
      echo "getting code from conjur"
     withCredentials([conjurSecretUsername(credentialsId: '807f6728-f34c-4ce2-8d1e-72b6c1dd63e2', passwordVariable: 'CONJUR_SECRET', usernameVariable: 'ManithejaCyberark')]) {
            git branch: 'master', credentialsId: '807f6728-f34c-4ce2-8d1e-72b6c1dd63e2', url: 'https://github.com/ManithejaCyberark/building-a-multibranch-pipeline-project.git'
           }
      }
   }
  stage("Deployed in production"){
    steps{
         echo "deployed completed"
      }
   }
 }
}
