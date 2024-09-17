pipeline{
    agent any

    stages{

        stage("git checkout stage"){
            steps{
                echo "checkout done"
                sh 'pwd'
            }
        }

        // stage("installing dependancies"){
        //     steps{
        //         sh ''
        //     }
        // }

        stage("cdk code deploy"){
            steps{
                sh 'cdk bootstrap'
                sh 'cdk apply'
            }
        }

        
    }
}