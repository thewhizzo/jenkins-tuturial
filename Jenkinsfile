pipeline{
        agent any
        stages{
            stage('Make Directory'){
                steps{
                    sh "mkdir ~/jenkins-tutorial-tester"
                }
            }
            stage('Make Files'){
                steps{
                    sh "touch ~/jenkins-tutorial-tester/file1 ~/jenkins-tutorial-tester/file2"
                }
            }
        }
}
