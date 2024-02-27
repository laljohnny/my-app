@Library("mylibs") _
pipeline {
  agent any
  tools {
    maven 'Maven'
  }
  stages{
    stage("Maven Build"){
      steps{
        bat "mvn clean package -Dv=${'Build_Number'} sonar:sonar"
      }
    }
    //stage("Deploy To Dev"){
     // steps{
      //  tomcatDeploy("tomcat-dev","ec2-user",["172.31.13.89","172.31.13.89"])
      //}
    //}
  }
}
