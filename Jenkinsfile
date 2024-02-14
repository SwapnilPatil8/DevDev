node {
    stage('Checkout') {
        git url: 'https://github.com/yourusername/yourrepository.git'
    }

    stage('Build') {
        // Add your build steps here
        sh 'mvn clean install'
    }

    stage('Test') {
        // Add your test steps here
        sh 'mvn test'
    }

    stage('Deploy') {
        // Add your deployment steps here
        // For example, deploying to a web server
        sh 'ssh user@server "cd /path/to/deploy && git pull"'
    }
}
