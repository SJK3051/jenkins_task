pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                git 'https://github.com/SJK3051/jenkins_task.git'
            }
        }

        stage('Run Ansible Playbook') {
            steps {
                sh 'ansible-playbook -i inventory deploy.yml'
            }
        }
    }
}
