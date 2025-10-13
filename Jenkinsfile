node('slave1') {
    stage('Source Code Checkout(Clone)') {
        git branch: 'main', url: 'https://github.com/Praveenkumar1290-janaki/Maven-java-project.git'
    }
    
    stage('Maven Build') {
        sh 'mvn clean package'
    }
}
