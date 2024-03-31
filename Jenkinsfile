pipeline {
    agent any
    options {
      buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '4', numToKeepStr: '4')
      disableConcurrentBuilds()
    }


    stages {
        stage('create some directories then delete them') {
            steps {
              sh '''
              mkdir fritz
              rm -rf fritz

              '''
                
            }
        }



        stage('create some files then delete them') {
            steps {
              sh '''
              touch esy
              rm -rf esy

              '''
                
            }
        }
    }
}
