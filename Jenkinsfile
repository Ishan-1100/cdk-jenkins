pipeline{
    agent any

    stages{

        stage("git checkout stage"){
            steps{
                echo "checkout done"
                sh 'pwd'
            }
        }

        stage("installing dependancies"){
            steps{
                sh 'whoami'
                sh 'sw_vers'
                //sh 'npm -v'
                // sh 'npm i -g aws-cdk typescript'
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
