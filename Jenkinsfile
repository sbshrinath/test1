pipeline {
     agent any

     stages {
          stage('Checkout') {
              steps {
                       checkout scm 
                    }
                            }
          stage('Build') {
              steps {
                      sh '/home/remote/Documents/software/apache-maven-3.9.6/bin/mvn install'
                    }
                         }
          stage('Deployment') {
              steps {
                      sh 'cp target/test1.war /home/remote/Documents/software/apache-tomcat-9.0.86/webapps'
                    }
                              }
            }
        }
 
        
