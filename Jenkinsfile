pipeline {

    agent any

    stages{
        stage('etapa de construccvión de la aplicación'){
            agent{
                docker{
                    image:'node:alpine3.20'
                }
            }
            stages("Install"){
                stage{
                    steps{
                        step{
                            sh 'npm install'
                        }
                    }
                }
            }
            stages("Echo del mensaje"){
                steps{
                  echo 'hola mundo'
                  sh 'echo "hola mundo desde el terminal"'
                }
        }
       
    }
}