pipeline {
    agent any
    
    stages {
        stage('Install SonarQube using Docker') {
            steps {
                script {
                    // Run Ansible playbook
                    ansiblePlaybook(
                        playbook: 'Playbook.yaml',
                        inventory: 'aws_ec2.yaml',
                       
                    )
                }
            }
        }
    }
}
