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

        

  }

}


