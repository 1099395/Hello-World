node {
  def mvnHome = tool 'maven3'
  def dockerHome = 'C:/docker'
  stage ("Intial Preparation") {
    bat "echo Preparations are done"
  }
   stage ("Build Code") {
     bat "cd C:\\Users\\1197316\\Downloads\\Sample\\Sample && ${mvnHome}/bin/mvn clean package"
     bat "echo code is builded"
   }
  stage ("Build image") {
   bat "cd C:\\Users\\1197316\\Downloads\\Sample\\Sample &&  ${mvnHome}/bin/mvn clean docker:build"
    bat "echo XXXXXXXXXX"
  }
   }
