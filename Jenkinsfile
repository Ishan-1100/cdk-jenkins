pipeline{
    agent any
    tools{
        nodejs "nodejs"
    }

    stages{


        stage("installing dependancies"){
            steps{
                
                sh 'npm version'
                
                // sh 'npm install'
                //sh 'npm version'
                // sh 'npm i -g aws-cdk typescript'
                sh 'tsc -v'
                
                // sh 'npm install'
                // sh 'apt install nodejs npm' 
                // sh 'npm install -g aws-cdk'
            }
        }

        stage("cdk code deploy"){
            steps{
                sh 'cdk --version'
                // sh 'aws --version'
                // sh 'cdk bootstrap'
                //sh 'cdk deploy -y'
                sh ' yes | cdk destroy'
            }
        }

        
    }

}
