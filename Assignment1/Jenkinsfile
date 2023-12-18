pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                script {
                    // Check out code from the Develop branch
                    checkout([$class: 'GitSCM', branches: [[name: '*/develop']], userRemoteConfigs: [[url: 'https://github.com/akhileshranjan2308/assignment1']]])

                    // Navigate to the directory containing the Jenkinsfile
                    dir('https://github.com/akhileshranjan2308/assignment1/Jenkinsfile') {
                        // Your steps here
                    }
                }
            }
        }

        // ... (other stages)
    }
}
