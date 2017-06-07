node {
  def mvnHome = tool 'maven3'
  def dockerHome = 'C:/Program Files/Docker Toolbox'
  stage ("Intial Preparation") {
    bat "echo Preparations are done"
  }
   stage ("Build Code") {
     bat "cd C:\\Drishya\\Hello-World-master\\Sample && ${mvnHome}/bin/mvn clean package"
     bat "echo code is builded"
   }
   }
