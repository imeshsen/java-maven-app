pipeline{
agent any

 stages{
  stage("clean up"){
   steps{
   deleteDir()
   }
  }
  stage("Clone"){
   steps{
   sh "git clone https://github.com/imeshsen/java-maven-app.git" 
   }
  } 
  stage("Build"){
   steps{
     sh "mvn clean package"
   } 
  }
  stage("Test"){
   steps{
     sh "mvn test"
   }
  } 
 }
}
