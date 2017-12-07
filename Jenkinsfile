node {
    checkout scm
    stage('Build') {
        echo 'Building..'
        sh 'npm install'
		sh 'npm run startpostgres && sleep 10 && npm run migratedb'
		sh 'npm testCI'
    }
    stage('Test') {
        echo 'Testing..'
    }
    stage('Deploy') {
        echo 'Deploying....'
    }
}




