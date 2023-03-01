pipeline{
  agent any
  
  stages{
  
    stage('build'){
      steps{
        sh 'mvn validate'
        echo 'Validated'
        }
      }
      stage('test'){
      steps{
        sh 'mvn test'
        echo 'Tested'
        }
      }
      stage('package'){
      steps{
        sh 'mvn package'
        echo 'Tested'
        }
      }
      
    }
}
