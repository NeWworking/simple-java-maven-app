pipeline{
    agent{
    label 'agent1'
    }
    environment{
     a="10"
    }
    maven{
    label 'maven323'
    }
    stages{
    stage('build'){
    sh 'mvn -version'
    sh 'mvn clean install'
    }
    stage('post build'){
    sh 'echo "build is successful"'
      }
      }
      }
