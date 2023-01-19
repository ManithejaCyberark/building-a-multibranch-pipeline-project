node {
  stage("git clone"){
     echo "git clone"
  }
  
  stage("git stage 2"){
     echo "stage2"
  }
  stage('Publish') { 
     withCredentials([conjurSecretCredential(credentialsId: 'WEB_PASSWORD', variable: 'CONJUR_SECRET')]) {
   echo "$CONJUR_SECRET"
    git branch: 'main', credentialsId: 'WEB_PASSWORD', url: 'https://github.com/ManithejaCyberark/building-a-multibranch-pipeline-project.git'
    }
//     withCredentials([conjurSecretCredential(credentialsId: 'folder_level_1_jenkins-app/db_password', variable: 'CONJUR_SECRET')]) {    
//       git branch: 'main', credentialsId: 'folder_level_1_jenkins-app/db_password', url: 'https://github.com/ManithejaCyberark/building-a-multibranch-pipeline-project.git'
//       echo "$CONJUR_SECRET"
//   }
  }
//     withCredentials([conjurSecretCredential(credentialsId: 'jenkins-app/db_password_globel_level', variable: 'CONJUR_SECRET')]) {
//      git branch: 'master', credentialsId: 'jenkins-app/db_password_globel_level', url: 'https://github.com/ManithejaCyberark/building-a-multibranch-pipeline-project.git'
//       echo "publish"
//     }    
//   }
}

