pipeline {
    agent any   
    stages {       
        stage('cloning Git') {
            steps {
                checkout scm
            }
        }
        stage('ansible Deploy') {
            steps {
                sh "ansible-playbook dockerimm.yml"               
            }
        }        
    }
}
