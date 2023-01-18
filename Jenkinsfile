node {
  stage('Publish') { 
    withCredentials([conjurSecretCredential(credentialsId: 'global_level_1_jenkins-app/db_password', variable: 'CONJUR_SECRET')]) {    
      git branch: 'main', credentialsId: 'global_level_1_jenkins-app/db_password', url: 'https://github.com/ManithejaCyberark/building-a-multibranch-pipeline-project.git'
      echo "$CONJUR_SECRET"
  }
 }
//     withCredentials([conjurSecretCredential(credentialsId: 'jenkins-app/db_password_globel_level', variable: 'CONJUR_SECRET')]) {
//      git branch: 'master', credentialsId: 'jenkins-app/db_password_globel_level', url: 'https://github.com/ManithejaCyberark/building-a-multibranch-pipeline-project.git'
//       echo "publish"
//     }    
//   }
}
