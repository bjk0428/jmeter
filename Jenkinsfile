// pipeline {
//     agent {
//         docker { image 'brainer:5000/jmeter' }
//     }
//     stages {
//         stage('Test') {
//             steps {
//                 sh 'jmeter --version'
//             }
//         }
//     }
// }

pipeline {
    agent {
        docker {
            image 'jmeter'
            args '-p 1099:1099'
        }
    }
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'jmeter --version'
            }
        }
        
    }
}