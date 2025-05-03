pipeline{
  agent any
  tools {maven "mavenV3"}

  stages{
    stage("checkout"){

      
      steps{
        git branch: "main" , url:"https://github.com/Amr-tmorot/SpringRESTful.git"
      }
    }

    stage("build"){

      steps{
        sh "mvn compile"
      }
    }


    stage("testt"){

      steps {
        
         sh "mvn test"
      }
    }
  }
}
