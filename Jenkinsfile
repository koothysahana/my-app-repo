pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '''
                  echo "Building project..."
                  mkdir -p build
                  echo "Hello World App" > build/app.jar
                  ls -l build/
                '''
            }
        }

        stage('Upload to JFrog (Simulated)') {
            steps {
                sh '''
                  echo "Pretending to upload build/app.jar to JFrog..."
                  echo "Using credentials: artifactory-creds (simulated)"
                  echo "Target repo: my-repo-local"
                  echo "Upload complete ✅"
                '''
            }
        }
    }
}
