node {
    checkout scm
    stage('Build') {
        echo 'Building..'
        sh 'npm install'
        sh 'cd client && npm install'
		sh 'npm run startpostgres && sleep 10 && npm run migratedb'
		sh 'npm run testCI'
    }
    stage('Build Docker'){

        sh './dockerbuild.sh'
    }
    stage('Test') {
        echo 'Testing..'
    }
    stage('Deploy') {
        echo 'Deploying....'
    }
}




