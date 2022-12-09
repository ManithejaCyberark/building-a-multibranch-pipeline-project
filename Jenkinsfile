pipeline {
 agent any
 stages{
   stage("fetch the code"){
    steps{
         echo "git clone completed"
      }
   }
  stage("clone from another repository"){
    steps{
        git branch: 'JenkinsCI_Issue', url: 'https://github.com/cyberark/ansible-conjur-collection.git'
        echo "cloned the another repo to mbp"
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
