node {
    checkout scm
    stage('Build') {
        echo 'Building..'
        npm install
		npm run startpostgres && sleep 10 && npm run migratedb
		npm testCI
    }
    stage('Test') {
        echo 'Testing..'
    }
    stage('Deploy') {
        echo 'Deploying....'
    }
}




