pipeline{

    agent any

    stages{

        stage('Git Checkout'){

            steps{

                script{

                    git branch: 'main', url: 'https://github.com/kennymath/java-project-app2.git'
                }
            }
        }
    }
}