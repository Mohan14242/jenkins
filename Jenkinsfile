pipeline{
    agent { node { label 'centos' } }

    stages{
        stage('Build') {
            steps {
                echo "building"
                sh "pwd"
            }
        }
       
        stage('Test') {
            steps {
                echo "this is the mohan test"
            }
        }

        stage('deploy') {
            steps {
                echo "deploying the succesful production to the test"
                
            }
        }
        stage('nothing'){
            steps {
                echo "this is for just testing the web hook"
            }
        }
    }

    post{
        always {
            echo " i willalways run  wheather job fails or pass i dont matter"
        }
        success{
            echo "i will run onyl when the pipeline is success"
        }
        failure{
            echo " i will run only when the  pipeline fails"
        }
    }
    
}