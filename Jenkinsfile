node {
  def mvnHome = tool 'maven3'
  def dockerHome = 'C:/Program Files/Docker Toolbox'
 stage ("Intial Preparation") {
    git credentialsId: 'github-creds', url: 'https://github.com/1099395/Hello-world'
  }
   stage ("Build Code") {
     bat "cd ${workspace}\\Sample && ${mvnHome}/bin/mvn clean package"
     bat "echo code is builded"
   }
    stage ("Build image"){
    bat "cd ${workspace} && docker_build.bat ${mvnHome}"
    bat "echo image is builded"
  }

   }
