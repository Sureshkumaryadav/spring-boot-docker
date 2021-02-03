/*node{
   stage('SCM Checkout'){
      
      git 'https://github.com/Sureshkumaryadav/spring-boot-docker'
    } 
    stage('Compile-Package'){
        def os = System.properties['os.name'].toLowerCase()
         echo "OS: ${os}"
         if (os.contains("linux")) {
            sh "mvn install" 
         } else {
            bat "mvn install"
         }
    }
}

*/

pipeline {

    agent any
    tools {
        maven 'Maven_3.6.3' 
    }
    stages {
       stage('SCM Checkout'){
      
      git 'https://github.com/Sureshkumaryadav/spring-boot-docker'
    } 
        stage('Compile stage') {
            steps {
                bat "mvn clean compile" 
        }
    }

         stage('testing stage') {
             steps {
                bat "mvn test"
        }
    }

          stage('deployment stage') {
              steps {
                bat "mvn deploy"
        }
    }

  }

}
