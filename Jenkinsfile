pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ PES1UG20CS325.cpp -o PES1UG20CS325'
                 build job: 'PES1UG20CS325-1', wait: false
                 echo 'Build by PES1UG20CS325 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat PES1UG20CS325.cpp'
                echo 'Test by PES1UG20CS325 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Deploy by PES1UG20CS325 successful'
            }
        }
    }

    post {
        failure {
            
                echo 'PES1UG20CS325 Pipeline Failed'
          
        }
    }
}
