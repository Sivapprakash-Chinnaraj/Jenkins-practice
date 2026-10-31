pipeline{
    agent any
    
    stages{
        stage("Vanakkam"){
            steps{
                echo 'Vaazhga paathi valamudan!'
                sh 'whoami'
                sh 'date'
                sh 'hostname'
            }
        }
        stage('Build'){
            steps{
                echo 'Application Built'
                sh 'pwd'
                sh 'python3 --version'
            }
        }
    }
    post{
        success{
            echo 'Pipeline built'
        }
        failure{
            echo 'Pipeline Failed to build'
        }
    }
}
