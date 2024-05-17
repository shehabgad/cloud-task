pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git url: "https://github.com/shehabgad/cloud-task.git", branch: 'master'
            }
        }
        stage('Execute Bash Script') {
            steps {
                sh 'chmod +x ./list_files.sh'
                sh './list_files.sh'
            }
        }
    }
}