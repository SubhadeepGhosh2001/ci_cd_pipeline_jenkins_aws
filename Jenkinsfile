node{
    def appDir = "/var/lib/jenkins/workspace/ci_cd_pipline_jenkins_aws"
    
    stage('Clean Workspace'){
        echo "Cleaning Workspace"
        deleteDir()
    }

    stage('Clone Repository'){
        echo "Cloning Repository"
        git(branch: 'main', url: 'https://github.com/sahil-kumar-123/ci_cd_pipline_jenkins_aws.git')
    }

}