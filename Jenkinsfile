pipeline{
        environment{
        a="10"
    }
    tools{
        maven 'maven363'
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
