pipeline{

    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                script {
                    // Simulate a build process
                    def buildResult = sh(script: 'echo "Build successful"', returnStatus: true)
                    if (buildResult != 0) {
                        error('Build failed!')
                    }
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                script {
                    // Simulate a test process
                    def testResult = sh(script: 'echo "Tests passed"', returnStatus: true)
                    if (testResult != 0) {
                        error('Tests failed!')
                    }
                }
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                script {
                    // Simulate a deployment process
                    def deployResult = sh(script: 'echo "Deployment successful"', returnStatus: true)
                    if (deployResult != 0) {
                        error('Deployment failed!')
                    }
                }
            }
        }
    }

    post {
        always {
            echo 'This will always run after the stages.'
        }
    }
}