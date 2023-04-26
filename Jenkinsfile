@Library('my-shared-library1') _

pipeline{

    agent any

    stages{

        stage('Git Checkout'){

            steps{

             gitCheckout(
                branch: "main",
                url: "https://github.com/kennymath/java-project-app2.git"

            )
            }


        }
        stage('Unit Test maven'){

            steps{

                script{

                    mvnTest()
                }
            }
        }
        stage('Integration Test maven'){
            steps{

                script{

                    mvnIntegrationTest()
                }
            }
        }

    }
}