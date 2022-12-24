pipeline {
    agent any
    stages{
        stage('vcs') {
            steps {
                git branch: 'dev', url: 'https://github.com/AnasAnsar1/react-storefront.git'
            }
        }
        stage('Image_build_and_Push') {
            steps {
                sh 'docker image build -t anasansarii/react-storefront:jnkdev'
                sh 'docker image push anasansarii/react-storefront:jnkdev'
            }
        }
    }
}