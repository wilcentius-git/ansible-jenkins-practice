pipeline {
    agent any
    environment {
        ANSIBLE_HOST_KEY_CHECKING = 'False'
    }
    stages {
        stage('Deploy') {
            steps {
                sh 'ansible-playbook -i inventory.ini hello.yml'
            }
        }
    }
}
