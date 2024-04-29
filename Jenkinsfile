node {

        stage('Build') {
            echo 'Building..'
            echo "${env.JOB_NAME}"
            echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
            sh '''
                echo ${env.JOB_NAME}
            '''
            sh '''
                echo "${env.JOB_NAME}"
            '''
        }
        stage('Test') {
            echo 'Testing..'
        }
        stage('Deploy') {
            echo 'Deploying....'
        }

}