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
<<<<<<< HEAD
                
                script {
                        sh """\
                            newman run ${testProjectJSON} -e ${testEnvironmentJSON}
                            """
                    }
                
=======
>>>>>>> branch 'dev' of git@github.com:gchuso/multibranch-pipeline.git
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
