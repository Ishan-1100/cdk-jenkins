pipeline{
    agent any
    tools{
        nodejs "nodejs"
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
                sh 'npm i -g aws-cdk typescript'
                sh 'tsc -v'
                sh 'cdk --version'
                // sh 'apt install nodejs npm' 
                // sh 'npm install -g aws-cdk'
            }
        }

        // stage("cdk code deploy"){
        //     steps{
        //         sh 'cdk bootstrap'
        //         sh 'cdk apply'
        //     }
        }

        
    }
