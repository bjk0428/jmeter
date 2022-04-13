// pipeline {
//     agent {
//         docker { image 'brainer:5000/jmeter' }
//     }
//     stages {
//         stage('Test') {
//             steps {
//                 ehco 'jmeter --version'
//             }
//         }
//     }
// }

pipeline {
    agent {
        docker { image 'node:16.13.1-alpine' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}
