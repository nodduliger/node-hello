pipeline{

    agent any

    stages {

        stage("build") {

            steps {
            echo "building the application"
            sh 'npm i'
            sh 'npm run build'
            }

        }


        stage("deploying") {

            steps {
            echo "deploying the application"
	sh '''
	npm start
	'''

            }

        }

    }

}
