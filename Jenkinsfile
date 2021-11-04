pipeline {
    agent {
        docker {
            image 'maven:3.5.4' 
            args '-v /var/jenkins_home/workspace/maven/.m2:/root/.m2' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
        
    }
}
