pipeline{
   agent any
   stages{
      stage{
         steps{
            checkout([$class: 'GitSCM', 
          branches: [[name: "${env.branch}"]], 
    doGenerateSubmoduleConfigurations: false, 
    extensions: [[$class: 'CleanCheckout']], 
    submoduleCfg: [], 
    userRemoteConfigs: [[credentialsId: '3d5cdb37-6e90-465b-9b1d-527ae99e152d', url: 'https://github.com/Ritik180/devops-test.git']]
])
         }
      }
   }
}
