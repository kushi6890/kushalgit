def workspace;
node
{
    stage('checkout')
    {
     checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '762cc871-c349-4eec-8057-861c08b02469', url: 'https://github.com/kushi6890/kushalgit.git']]])
    workspace = pwd()
    }
    stage('static code analysis')
    {
        echo "static code analysis"
    }
    stage('build')
    {
        echo "build the code"
    }
    stage('unit testing')
    {
        echo "unit testing"
    }
    stage('delivery')
    {
        echo "deliver the code"
    }
    
}
