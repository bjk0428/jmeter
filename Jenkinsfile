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

node {
    docker.image('jmeter').withRun('-e "PATH=/usr/local/src/apache-jmeter-5.4.3/bin:$PATH" -d -p 1099:1099') { c ->
        docker.image('jmeter') {
 
            sh 'ehco jk'
        }
    }
}