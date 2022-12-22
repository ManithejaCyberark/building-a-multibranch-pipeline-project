pipeline {
 agent any
 stages{
   stage("fetch the code"){
    steps{
         withCredentials([conjurSecretUsername(credentialsId: 'dc69116a-9076-490a-a87a-55cd9e199b90', passwordVariable: 'CONJUR_SECRET', usernameVariable: 'ManithejaCyberark')]) {
                 echo "$CONJUR_SECRET"
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
