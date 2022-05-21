pipeline{
    agent any
    stages{
        stage("Build + UT"){
            steps{
                script{
                     sh 'mvn compile test'
                }
            }
        }
    }
    post{
        always{
            echo "========always========"
        }
        success{
            echo "========pipeline executed successfully ========"
        }
        failure{
            echo "========pipeline execution failed========"
        }
    }
}
