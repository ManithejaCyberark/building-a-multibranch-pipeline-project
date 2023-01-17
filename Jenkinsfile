pipeline {
 agent any
 stages{
   stage("Git Checkout"){
    steps{
      echo "getting code from conjur"
           withCredentials([conjurSecretCredential(credentialsId: 'f10717d6-2bd2-49c6-83d5-a0b9384b8fa6', variable: 'CONJUR_SECRET')]) {
             git branch: 'master', credentialsId: 'f10717d6-2bd2-49c6-83d5-a0b9384b8fa6', url: 'https://github.com/ManithejaCyberark/building-a-multibranch-pipeline-project.git'
           }
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
