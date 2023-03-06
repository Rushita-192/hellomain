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
    
    stage('Deploy to Nexus'){
      steps{
        sh 'mvn deploy -Dmaven.test.skip=true'
        echo 'Deployed Sucessfully...'
        }
      }
      
    }
}
