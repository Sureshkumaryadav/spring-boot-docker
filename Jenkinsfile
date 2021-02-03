node{
   stage('SCM Checkout'){
      
      git 'https://github.com/Sureshkumaryadav/spring-boot-docker'
    } 
    stage('Compile-Package'){
       //Get maven home path
       //def mvnHome = tool name: 'maven', type: 'maven'
       //sh 'mvn package'
        //Get maven home path
        def mvnHome = tool name: 'maven', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
    }
}

