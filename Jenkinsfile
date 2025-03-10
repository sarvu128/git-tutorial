pipeline{
    agent any
    stages{
        stage('Git-checkout'){
            steps{
                git changelog: false, poll: false, url: 'https://github.com/sarvu128/git-tutorial.git'
            }
        }
        stage('Build'){
            steps{
                bat 'build.bat'
            }
        }
        stage('Quality'){
            steps{
                bat 'quality.bat'
            }
        }
        stage('Deploy'){
            steps{
                bat 'deploy.bat'
            }
        }
    }
}
