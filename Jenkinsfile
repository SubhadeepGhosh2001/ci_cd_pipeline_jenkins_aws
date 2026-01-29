node{
    def appDir = "/var/lib/jenkins/workspace/ci_cd_pipline_jenkins_aws"
    
    stage('Clean Workspace'){
        echo "Cleaning Workspace"
        deleteDir()
    }

    stage('Clone Repository'){
        echo "Cloning Repository"
        git(branch: 'main', url: 'https://github.com/SubhadeepGhosh2001/ci_cd_pipeline_jenkins_aws')
    }

    stage('Deploy to EC2'){
        echo "Deploying to EC2"
        sh """
          sudo mkdir -p ${appDir}
          sudo chown -R jenkins:jenkins ${appDir}
          rsync -av --delete --exclude='.git' --exclude='node_modules' ./ ${appDir}/
          cd ${appDir}
          sudo npm install
          sudo npm run build
          sudo fuser -k 3000/tcp || true
          sudo npm run start
        """
    }

}