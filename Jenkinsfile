pipeline 
 {
  agent any
  stages{
  stage('Build Application'){
  steps{
  bat 'mvn clean install'
  }
  }
  
  stage('Deploy application to cloud'){
  steps{
  bat 'mvn package deploy -DmuleDeploy'
  }
  }
  
  stage('Run newman test cases for regression testing'){
  steps{
  bat 'C:\\Users\\snayeem\\AppData\\Roaming\\npm\\newman run C:\\Users\\snayeem\\Desktop\\collections\\worldtimezone.postman_collection.json --disable-unicode'
  }
  }
  
  }

 }