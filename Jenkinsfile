pipeline {
     triggers {
  pollSCM '* * * * *'
}
     agent any
    tools {
  maven 'M2_HOME'
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
        
        stage('deploy') {
            steps {
                echo 'deploy'
                sleep 5
            }
        }
    }
}