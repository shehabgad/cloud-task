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
                sh './list_files.sh'
            }
        }
    }
}