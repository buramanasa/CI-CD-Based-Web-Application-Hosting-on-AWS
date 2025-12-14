pipeline {
agent any
stages {
stage('Clone Repo') {
steps {
git 'https://github.com/your-username/ci-cd-aws-webapp.git'
}
}
stage('Build Docker Image') {
steps {
sh 'docker build -t aws-cicd-app .'
}
}
stage('Run Container') {
steps {
sh 'docker run -d -p 80:80 aws-cicd-app'
}
}
}
}
