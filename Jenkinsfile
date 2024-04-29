node {
        MY_JOB_NAME = "${env.JOB_NAME}"

        stage('Build') {
            echo 'Building..'

            echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
            sh """
                echo 'Job Name: ${env.JOB_NAME}'
            """
            echo "Job Name is ${env.JOB_NAME}"
            echo "$JOB_NAME"
            echo "${JOB_NAME}"
            sh '''
                echo "done" > /var/lib/jenkins/workspace/${JOB_NAME}/asdf.txt
            '''
        }
        stage('Test') {
            echo 'Testing..'
        }
        stage('Deploy') {
            echo 'Deploying....'
        }

}