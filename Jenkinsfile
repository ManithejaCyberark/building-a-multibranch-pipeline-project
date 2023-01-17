pipeline {
 agent any
 stages{
   stage("Git Checkout"){
    steps{
      echo "getting code from conjur"
     withCredentials([conjurSecretCredential(credentialsId: 'host_key_test_pipeline1', variable: 'CONJUR_SECRET')]) {
   git branch: 'master', credentialsId: 'host_key_test_pipeline1', url: 'https://github.com/ManithejaCyberark/building-a-multibranch-pipeline-project.git'
     }
   }
  stage("Deployed in production"){
    steps{
         echo "deployed completed"
      }
   }
 }
}
