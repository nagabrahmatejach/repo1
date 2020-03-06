def workspace;
node
{
    stage('checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'cc717e30-30a5-42cf-ba55-708ed56daf69', url: 'https://github.com/nagabrahmatejach/repo1.git']]])
        workspace =pwd()
    }
    stage('Static code analysis')
    {
        echo "Static code analysis"
    }
    stage('Build')
    {
        echo "Build the code"
    }
    stage ('Unit Testing')
    {
        echo "Unit testing"
    }
    stage ('Delivery')
    {
        echo "Delivery the code"
    }
}
