pipeline{
  agent any
  stages{
    stage("Bulid"){
      steps{
        script{
          echo 'building the project'
          bat 'mvn clean package'
        }
      }
    }
     stage("test"){
       steps{
         script{
           echo 'testing the project '
           bat 'mvn clean test'
         }
       }
    }
     stage("server"){
       steps{
         script{
            echo 'deploying the project '
            bat 'start mvn tomcat7:run'
         }
       }
    }
  }
}
