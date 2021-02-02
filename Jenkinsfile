pipeline{
    agent{
        label 'agent1'
    }
    environment{
        a="10"
    }
    tools{
        maven 'maven323'
    }
    stages{
        stage('build'){
            steps{
                sh "mvn -version"
                sh "mvn clean install"
            }
        }
        stage('post build'){
            steps{
                sh 'echo "build is successful: $a"'
            }
        }
    }
}
