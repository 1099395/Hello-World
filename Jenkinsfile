node {
  def mvnHome = tool 'maven3'
  def dockerHome = 'C:/Program Files/Docker Toolbox'
  stage ("Intial Preparation") {
    bat "echo Preparations are done"
  }
   stage ("Build Code") {
     bat "cd C:\\chaitra\\login-service && ${mvnHome}/bin/mvn clean package"
     bat "echo code is builded"
   }
   }
