node {
    stage('Source Code Checkout(Clone)') {
        git branch: 'main', url: 'https://github.com/Praveenkumar1290-janaki/Maven-java-project.git'
    }
    
    stage('Maven Build') {
        bat 'mvn clean package'
    }
        stage('sonarqube') {
   bat 'mvn sonar:sonar -Dsonar.projectKey=test -Dsonar.host.url=http://localhost:9000 -Dsonar.login=697b99198fcb96feeda9af4adf1ed16e0fc632c0'
    }
    
}
