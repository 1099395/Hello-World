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
    SET DOCKER_TLS_VERIFY=1
SET "DOCKER_HOST=tcp://192.168.99.103:2376"
SET "DOCKER_CERT_PATH=C:\\Users\\1099395\\.docker\\machine\\machines\\default"
SET "DOCKER_MACHINE_NAME=default"
SET "COMPOSE_CONVERT_WINDOWS_PATHS=true"
   bat "cd C:\\Users\\1197316\\Downloads\\Sample\\Sample && ${mvnHome}/bin/mvn docker:build"
    bat "echo XXXXXXXXXX"
  }
   }
