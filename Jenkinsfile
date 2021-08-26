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
                    sudo docker build .
                '''
            }
        }
        
}
        
}
             
