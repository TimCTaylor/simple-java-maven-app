pipeline {
    agent any
    tools { 
        maven 'maven-399'
    }
    options {
        timeout(time: 5, unit: 'MINUTES')   // timeout on whole pipeline job
    }

    stages {
        stage('Build') { 
            steps { sh 'mvn -B -DskipTests clean package' }
        }
    }
}
