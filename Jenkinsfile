pipeline{
  agent any
  
  stages{
  
    stage('build'){
      step{
        sh mvn validate
        echo Validated
        }
      }
      stage('test'){
      step{
        sh mvn test
        echo Tested
        }
      }
      stage('package'){
      step{
        sh mvn package
        echo Tested
        }
      }
      
    }

}
