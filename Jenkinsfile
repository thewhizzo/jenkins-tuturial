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
                    sh "touch ~/jenkins-tuturial/file1 ~/jenkins-tuturial/file2"
                }
            }
        }
}
