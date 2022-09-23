pipeline {
    agent any
    tools {
  maven 'M2_HOME'
}
    triggers {
  pollSCM '* * * * *'
}

    stages {
        stage('maven package') {
            steps {
                sh 'mvn clean'
                sh 'mvn install'
                sh 'mvn package'
                sleep 5
            }
        }
        stage('test') {
            steps {
                sh 'mvn clean'
                
            }
        }
        stage('test') {
            steps {
                echo 'test'
                
            }
        }
        stage('deploy') {
            steps {
                echo 'deploy'
                sleep 5
            }
        }
    }
}