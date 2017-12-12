node {
    checkout scm
    stage('Setup') {
        echo 'Setting up'
        sh 'npm install'
        sh 'cd client && npm install'
    }
    stage('Test') {
        echo 'Testing..'
        sh 'npm run testCI'
    }
    stage('Deploy') {
        echo 'Deploying....'
        sh './dockerbuild.sh'
        dir('./provisioning')
        {
            sh "./provision-new-environment.sh"
        }
    }
}




