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
                
                sh '''#!/bin/bash
                
                    echo " Hi, I am fine."
                    
                   '''
            }
        }
                 
           
    }
}
