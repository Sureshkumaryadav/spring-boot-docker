node{
   stage('SCM Checkout'){
      
      git 'https://github.com/Sureshkumaryadav/spring-boot-docker'
    } 
    stage('Compile-Package'){
       //Get maven home path
       //def mvnHome = tool name: 'maven', type: 'maven'
       sh 'mvn package'
    }
}

