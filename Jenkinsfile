pipeline
{
  agent any
  stages
  {
    stage('1')
    {
      steps
      {
       sh 'git clone https://github.com/RavitejaAdepudi/vamsi'
      }
    }
     stage('2')
    {
      steps
      {
       sh 'export MAVEN_HOME=/opt/apache-maven-3.9.9 && export PATH=$PATH:/opt/apache-maven-3.9.9/bin && mvn -f /var/lib/jenkins/workspace/mar12th1st/vamsi/mavewebappdemo/pom.xml install'
      }
    }
    stage('3')
    {
      steps
      {
       sh 'cp -R /var/lib/jenkins/workspace/mar12th1st/vamsi/mavewebappdemo/target/*.war /opt/apache-tomcat-9.0.100/webapps'
      }
    }
  }
}
