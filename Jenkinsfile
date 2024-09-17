pipeline{
    agent any
    tools{
        nodejs "nodejs"
    }
    
    environment {
        AWS_ACCESS_KEY_ID = credentials('aws_access_key_id_secret_id')
        // AWS_SECRET_ACCESS_KEY = credentials('aws_secret_access_key_secret_id')
    }


    stages{

        // stage("git checkout stage"){
        //     steps{
        //         echo "checkout done"
        //         sh 'pwd'
        //     }
        // }

        stage("installing dependancies"){
            steps{
                // sh 'ls'
                // sh 'whoami'
                // sh 'echo $PATH'
                sh 'npm version'
                // sh 'sudo -u jenkins which npm'
                // sh 'npm install'
                //sh 'npm version'
                // sh 'npm i -g aws-cdk typescript'
                sh 'tsc -v'
                sh 'cdk --version'
                sh 'npm install'
                // sh 'apt install nodejs npm' 
                // sh 'npm install -g aws-cdk'
            }
        }

        stage("cdk code deploy"){
            steps{
                // sh 'cdk bootstrap'
                sh 'echo "AWS_ACCESS_KEY_ID" ' ;
                //sh 'cdk deploy --require-approval never'
                
            }
        }

        
    }

}
