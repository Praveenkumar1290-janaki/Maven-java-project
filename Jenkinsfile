node {
    stage('Source Code Checkout(Clone)') {
        git branch: 'main', url: 'https://github.com/Praveenkumar1290-janaki/Maven-java-project.git'
    }
    
    stage('Maven Build') {
        bat 'mvn clean package'
    }
        stage('sonarqube') {
   bat 'mvn sonar:sonar -Dsonar.projectKey=bankpo -Dsonar.host.url=http://localhost:9000 -Dsonar.login=ee3ec93364cba01013e493970915ae679afd1574'
    }
    
}
