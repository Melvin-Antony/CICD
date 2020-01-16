pipeline {
    agent any

    stages {
         stage('checkout') {
           steps {
                    
                    git 'https://github.com/Melvin-Antony/CICD.git'
                 }  
        }
        stage('ansible') {
           steps {
                    
                    ansiblePlaybook become: true, inventory: 'hosts', playbook: 'deploy.yml'
                 }  
        }
    }
}
