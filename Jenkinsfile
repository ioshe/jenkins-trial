node {
        MY_JOB_NAME = "${env.JOB_NAME}"

        stage('Build') {
            echo 'Building..'

            echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
            sh """
                echo 'Job Name: ${env.JOB_NAME}'
            """
            sh '''
                echo '${MY_JOB_NAME}'
                env | grep MY_JOB_NAME
                #    echo 'Job Name: ${env.JOB_NAME}'
                # echo '${env.JOB_NAME}' => ${env.JOB_NAME} 문자열 그대로 나옴
                # 안됨 echo "${env.JOB_NAME}"
                # echo "${env.JOB_NAME}"
            '''
        }
        stage('Test') {
            echo 'Testing..'
        }
        stage('Deploy') {
            echo 'Deploying....'
        }

}