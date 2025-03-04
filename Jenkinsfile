pipeline {
    agent any

    stages {
        stage('Build') {
            agent {
                docker {
                    image 'node:18-alpine'
                    reuseNode true
                }
            }
            steps {
                    sh '''
                        mkdir build
                        npm run build

                    '''
            }
        }
    }
}