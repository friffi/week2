node {
    checkout scm
    stage('Build') {
        echo 'Building..'
        sh 'npm install'
		sh 'npm testCI'
    }
    stage('Test') {
        echo 'Testing..'
    }
    stage('Deploy') {
        echo 'Deploying....'
    }
}




