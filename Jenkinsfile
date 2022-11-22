pipeline{
        agent any
        stages{
            stage('Make Directory'){
                steps{
checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/thewhizzo/jenkins-tuturial.git']]])
                }
            }
            stage('Make Files'){
                steps{
                    sh "touch /home/jenkins/.jenkins/workspace/hack1-prep/file1 /home/jenkins/.jenkins/workspace/hack1-prep/file2"
                }
            }
        }
}
