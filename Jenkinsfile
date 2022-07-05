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
                sh "sudo ansible-playbook dockerimm.yml"               
            }
        }        
    }
}
