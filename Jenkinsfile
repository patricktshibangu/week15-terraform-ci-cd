pipeline{
    agent any
    stages{
        stage ('init'){
            steps {
                sh 'terraform init'
            }
        }
        stage ('format'){
            steps {
                sh 'terraform fmt'
            }
        }
        stage ('validate'){
            steps {
                sh 'validate'
            }
        }
        stage ('plan'){
            steps {
                sh 'terraform plan'
            }
        }
        stage ('apply'){
            steps {
                sh 'terraform apply --auto-approve'
            }
        }
        stage ('destroy'){
            steps {
                sh 'terraform destroy --auto-approve'
            }
        }
    }
}
