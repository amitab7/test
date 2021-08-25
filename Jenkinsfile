pipeline {
    agent none

    stages {

        stage ('Git') {
            agent any

            steps {
                
             sh '''#!/bin/bash

                    echo "Hello from bash"
                    echo "Who I'm $SHELL"
                    echo " Hello World!"
                    echo " How are you ?"
                '''
            }
        }
        stage ('Docker'){
            agent any
            steps {
                
                stages {
        stage('build and push') {
            when {
                branch 'master'
            }
            sh "docker build -t docker/getting-started ."

            steps {
                withDockerRegistry([url: "", credentialsId: "dockerbuildbot-index.docker.io"]) {
                    sh("docker push docker/getting-started")
                }
            }
        }
    }
}

            }
        }
                 
           
    }
}
