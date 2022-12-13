stages {
    stage('Checkout GIT') {
        steps {
            echo 'Pulling .....';
            git branch : 'youssef-back',
            url : 'https://github.com/farouk-hajjej/Devops-Projet-5SE1.git'
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
             
                   

 }
