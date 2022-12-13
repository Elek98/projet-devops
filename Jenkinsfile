pipeline {
    agent any

stages {
    stage('Checkout GIT') {
        steps {
            echo 'Pulling .....';
            git branch : 'ahmed_branch',
            url : 'https://github.com/Elek98/projet-devops.git'
        }
                          }
        

    stage('MVN CLEAN'){
                 steps{
                     sh  'mvn clean install -U'
                 }
                           }
    stage('MVN COMPILE'){
            steps{
                sh  'mvn compile'
                 }
                            }
     stage('MVN PACKAGE'){
            steps{
                sh  'mvn package'
                      }
                                  }
          stage('MVN SONARQUBE'){
                         steps{
                                sh  'mvn sonar:sonar -Dsonar.login=admin -Dsonar.password=ahmed2077'
                         }
                   }
                   

 }
}
