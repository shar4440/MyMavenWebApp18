pipeline{
  ageny any

  tools{
    maven 'Maven'
    jdk   'JDK'
  }

  stages{
    stage('Checkput'){
      steps{
         git branch: 'master',url : 'https://github.com/shar4440/MyMavenWebApp18.git'
      }
    }

    stage('Buildd'){
      steps{
        sh 'mvn clean package'
      }
    }

    stage('Running'){
      steps{
        sh '''
          #hgxvx uydgukghc
          sudo 'cp /home/shruthi/Desktop/dev2/MyMavenWebApp18/target/MyMavenWebApp18.war /opt/tomcat/webapps/'
          '''
      }
    }
  }
}
