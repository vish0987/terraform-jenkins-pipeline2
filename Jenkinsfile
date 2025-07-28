pipeline {
   agent any
   
   stages {
        stage('Clone Repo') {
            steps {
              git branch: 'main' , url : 'https://github.com/vish0987/terraform-jenkins-pipeline2.git'
              }
           }
        stage('terraform init') {
            steps {
               sh 'terraform init'
              }
            }
        stage('terraform validate') {
            steps {
               sh 'terraform validate'
              }
            }
        stage('terraform plan') {
            steps {
               sh 'terraform plan'
              }
            }
        stage('terraform apply') {
            steps {
               sh 'terraform apply -auto-approve'
              }
            }
}
}
