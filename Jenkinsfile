
testProjectJSON = 'postman/collection.json'
testEnvironmentJSON = 'postman/environment.json'

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                
                script {
                        sh """\
                            newman run ${testProjectJSON} -e ${testEnvironmentJSON} --insecure
                            """
                    }
                
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
