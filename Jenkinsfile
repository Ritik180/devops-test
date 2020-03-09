node{ 
   checkout([$class: 'GitSCM', 
          branches: [[name: "${env.branch}"]], 
    doGenerateSubmoduleConfigurations: false, 
    extensions: [[$class: 'CleanCheckout']], 
    submoduleCfg: [], 
    userRemoteConfigs: [[credentialsId: 'git-credentials', url: 'https://github.com/user/repo.git']]
])
       }
