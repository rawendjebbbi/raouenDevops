pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                echo 'salut'
            }
        }
        stage('Git'){
            steps{
                echo 'pulling from git ....';
                git branch :'master', url:'https://github.com/mhassini/timesheet-devops.git'; 
            }
        }
        stage('maven'){
            steps{
                echo 'building project...';
                sh 'mvn -version';
            }
        }
    }
}
