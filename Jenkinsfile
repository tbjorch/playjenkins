pipeline{
    agent any
    /*tools {
        maven: 'maven3'
        jdk8: 'OracleJDK1.8'
    }*/
    stages{
        parallel {
            stage("A"){
                steps{
                    echo "========executing A after changing stuff in my repo AND TESTING AGAING ========"
                }
                post{
                    always{
                        echo "========always========"
                    }
                    success{
                        echo "========A executed successfully ========"
                    }
                    failure{
                        echo "========A execution failed========"
                    }
                }
            }
            stage("B"){
                steps{
                    echo "========executing B after changing stuff in my repo AND TESTING AGAING ========"
                }
            }
            stage("C"){
                steps{
                    echo "========executing C after changing stuff in my repo AND TESTING AGAING ========"
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