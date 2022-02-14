pipeline {
    agent any
    environment{
        PATH="/opt/maven3/bin:$PATH"
    }
    stages{
        stage('Git'){
            steps{
                git changelog: false, poll: false, url: 'https://github.com/logeshSLK/Rahulshetty'
            }
        }
        stage('MAVEN'){
            steps{
                sh 'mvn clean package'
            }
        }
        
    }
}
