//Jenkins pipeline script
//Groovy script 

node{
  def mavenHome = tool name: 'maven3.9.4'
  stage('CodeClone') {
    git credentialsId: 'git-credentials', url: 'https://github.com/DirandU21/maven-web-apps.git'
  }
  stage('mavenBuild') {
    sh "${mavenHome}/bin/mvn clean package"
  }
/*
  stage('CodeQuality') {
    sh "${mavenHome}/bin/mvn sonar:sonar"
  // execute the CodeQuality report with sonar
  }
  stage('emailQualityIssues') {
    emailext body: '''Thanks

Itech Solutions''', recipientProviders: [developers()], subject: 'status of build', to: tosomisaac7@gmail.com'
  }

   stage('UploadNexus') {
    sh "${mavenHome}/bin/mvn deploy"
    //mvn deploy  are uploaded in to nexus
  }

  stage('DeployTomcat') {
    deploy adapters: [tomcat9(credentialsId: 'tomcat', path: '', url: 'http://34.239.155.145:7000/')], contextPath: null, war: 'target/*war'
  }
  stage('emailDeployIssues') {
    emailext body: '''Thanks

Itech Solutions''', recipientProviders: [developers()], subject: 'status of build', to: 'tosamisaac7@gmail.com'
  }
 */ 
}
