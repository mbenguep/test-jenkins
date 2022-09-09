node{
    stage('Checkout'){
        git 'https://github.com/mbenguep/test-jenkins'
    }
    stage('compile-package'){

        sh "/usr/bin/mvn package"
    }
    stage('SonarQube Analysis') {
        echo 'Code Quality'
        withSonarQubeEnv('sonar-1') { 
          sh "/usr/bin/mvn clean sonar:sonar"
        }
    }


}