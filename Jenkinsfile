pipeline {
    agent {
        docker { image 'brainer:5000/jmeter' }
    }
    stages {
        stage('Test') {
            steps {
                ehco 'jmeter --version'
            }
        }
    }
}

