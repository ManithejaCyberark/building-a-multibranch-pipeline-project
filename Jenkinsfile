pipeline {
 agent any
 stages{
   stage("fetch the code"){
    steps{
         withCredentials([conjurSecretCredential(credentialsId: 'test-pipeline-credential2', variable: 'CONJUR_SECRET')]) {
           // some block
         }
      }
   }
    stage("build"){
    steps{
         echo "build completed"
      }
   }
  stage("Deployed in production"){
    steps{
         echo "deployed completed"
      }
   }
 }
}
