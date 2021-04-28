pipeline
 {
  agent any
   stages{
    stage('Build Application'){
    steps{
    bat 'mvn clean install'
    }
    }
    
    stage('Deploy'){
    steps{
    bat 'mvn package deploy -DmuleDeploy'
    }
    }
    
    stage('Perform Testing'){
    steps{
    bat 'newman run C:\Users\hp\Documents\newman\mule-jenkins-test.postman_collection.json --disable-unicode'
    }
    }
   
   }


 }