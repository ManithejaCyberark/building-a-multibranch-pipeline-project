pipeline {
 agent any
 stages{
   stage("Git Checkout"){
    steps{
      echo "getting code from conjur"
//         git credentialsId: 'a86a704c-802f-40ce-b51f-db29c6ad38cc', url: 'https://github.com/ManithejaCyberark/conjur-quickstart.git'
//           echo "getting code from conjur"
         
//         withCredentials([conjurSecretCredential(credentialsId: 'test-pipeline-credential2', variable: 'CONJUR_SECRET')]) {
//            echo "conjur provided credential $CONJUR_SECRET"
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
