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
            args '-e PATH=/usr/local/src/apache-jmeter-5.4.3/bin:$PATH -it -p 1095:1099 —name jmeter -v /usr/local/src/docker_jmeter/apache-jmeter-5.4.3:/usr/local/src'
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