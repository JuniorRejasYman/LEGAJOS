pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'mvn clean package'
      }
    }

    stage('test') {
      steps {
        sh 'mvn test'
      }
    }

    stage('builds') {
      steps {
        sh 'cp /root/.jenkins/workspace/AS2017S6_Legajos_Java_Dev/target/Legajos.war /opt/wildfly/standalone/deployments'
      }
    }

  }
}