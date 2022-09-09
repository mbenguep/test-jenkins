node{
    stage('Checkout'){
        git 'https://github.com/mbenguep/test-jenkins'
    }
    stage('compile-package'){

        sh "usr/bin/mvn package"
    }


}