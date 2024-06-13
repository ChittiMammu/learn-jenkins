pipeline {
    agent AGENT1
    stages {
        stage('Example') {
            agent AGENT1
            options {
                // Timeout counter starts BEFORE agent is allocated
                timeout(time: 1, unit: 'SECONDS')
            }
            steps {
                echo 'Hello World'
            }
        }
    }
}